<template>
    <div>
        <div class="pb-5">
		<div class="container text-center">
			<img class="img-fluid" src="static/img/header-img.png" alt="É dividindo o bolo que se faz a festa">

			<h2 class="font-FlamaLight text-secondary">Obrigado pela sua participação!</h2>
			
		</div>
		
			<footer>
				<h4 class="font-FlamaLight text-secondary text-center">Redirecionando ...</h4>
			</footer>
		</div>
    </div>
    
</template>

<script>
import axios from 'axios';
import qs from 'qs';
// Import component
import Loading from 'vue-loading-overlay';
// Import stylesheet
import 'vue-loading-overlay/dist/vue-loading.css';
	
export default {
    name: 'agradecer',
    data() {
        return {
            msg: 'Welcome to Your Vue.js App',
            isLoading: false,
            fullPage: true,
			listInstitute: [ 'ABRIGO MOACYR ALVES',  'ABRIGO O CORACAO DO PAI', 'LAR DAS MARIAS', 'ABRIGO NACER']
        };
    },
    components: {
        Loading,
    },
    methods: {
        doar(idInstitute) {
            console.log('asd', idInstitute);
            this.doVote(idInstitute);
        },
        async doVote(idInstitute) {
			this.isLoading = true;
            await axios
                .post(
					'http://10.0.8.107:3000/institute/vote', // host
                    qs.stringify({ institute: idInstitute }), // dados
                    {
                        headers: {
                            'Content-Type': 'application/x-www-form-urlencoded',
                        },
                    }
                )
                .then( async (result) => {
					if (result.data){
						let thanks = await this.loadThanks()
						
						
                        window.location.href = `http://192.168.6.251:8080/agradecer/?ds_senha=${thanks.DS_AGRADECIMENTO.replace(/ /g, '$')}&nm_nome=${thanks.NM_PESSOA_AGRADECIMENTO}&nm_institute=${this.listInstitute[ idInstitute - 1 ].replace(/ /g, '$' )} `;
					}
					return result
				})
				.finally(() => {
					this.isLoading = false
				})
                .catch((err) => {
                    console.log('Erro ao registar o voto.', err);
                });
        },
        loadThanks() {
			return axios.get(`http://10.0.8.107:3000/thanks/${ Math.floor(Math.random() * (5 - 1 + 1 )) +1 }`)
			.then((res) => {
                if ( res.data )  {
					return res.data[0]
				}
            });
        },
    },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
 footer {
	bottom: 0px;
	position:absolute ;
	margin:  auto;
 }
</style>
