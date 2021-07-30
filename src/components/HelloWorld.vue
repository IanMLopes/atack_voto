<template>
    <div class="page">
        <div class="pb-5">
		<!-- <div class="container text-center"> -->
			<!-- <img class="img-fluid" src="static/img/header-img.png" alt="É dividindo o bolo que se faz a festa"> -->

			<!-- <h2 class="font-FlamaLight text-secondary">E aí? Pra qual Instituição você vai doar a sua fatia do bolo?</h2> -->
			<!-- <p class="h3 font-FlamaBold text-secondary font-weight-bold">ESCOLHA SUA INSTITUIÇÃO AQUI:</p> -->
		<!-- </div> -->
		<!-- -->
		<div class="container pb-1" style=" margin-bottom:5px; border: 1px solid red !important">
			<div class="row" >
				<div class="col-md-6" style="width: 60% !important">
					<img class="img-fluid w-100" src="static/img/moacyr-alves.png" alt="ABRIGO MOACYR ALVES">
					<div class="bg-info text-white py-2 px-4 " style="background: #ffcc00 !important">
						<h2 class="h4 m-0 font-weight-bold font-FlamaBold" style="color: #2F2F2F">ABRIGO MOACYR ALVES</h2>
						<h2 class="h5 m-0 font-weight-bold font-FlamaBold" style="color: #2F2F2F; text-align: justify;">Atende crianças com deficiências.</h2>
						<p class="m-0" style="color: red; font-weight: bold">Rua Professora Lea Alencar, 1014 - Alvorada</p>
						<p class="m-0" style="color: red; font-weight: bold">Fone: (92) 3238-2112</p>
					</div>
				</div>
				<div class="col-md-5 text-center">
					<p class="h3 font-weight-bold font-FlamaBold" style="color: #cc0000; text-align: left">Quer saber mais?</p>
					
					<p class="h5 font-FlamaBold" style="color: #696969; text-align: left">Aponte seu celular e conheça o trabalho desta instituição.</p>
					<div style="display: flex !important">
						<div>
							<img class="img-fluid my-4" src="static/img/moacyr-qr-code.jpg" alt="ABRIGO MOACYR ALVES">
						</div>
						<div @click.prevent="doar(1)" style="background: #cc0000; width: 180px; height: 110px; margin-left:10px; margin-top: 40px; cursor: pointer;" >
					<a href="" 
                        
                        class="  font-weight-bold    w-70  text-white" style=" font-size:35px;  !important; bottom: 5px !iportant; line-height: 50px;">QUERO DOAR! </a>
					</div>
					</div>	
				</div>
			</div>
		</div>
		<!-- -->
		<div class="container pb-1" style="border: 1px solid red !important; margin-bottom:5px; ">
			<div class="row">
				<div class="col-md-6">
					<img class="img-fluid w-100  " src="static/img/abrigo-coracao-do-pai.png" alt="ABRIGO O CORAÇÃO DO PAI">
					<div class="bg-info text-white py-2 px-4 " style="background: #ffcc00 !important">
						<h2 class="h4 m-0 font-weight-bold font-FlamaBold" style="color: #2F2F2F">ABRIGO O CORAÇÃO DO PAI</h2>
						<h2 class="h5 m-0 font-weight-bold font-FlamaBold" style="color: #2F2F2F; text-align: justify;">Acolhendo crianças resgatadas de situações de alto risco pessoal</h2>
						
						<p class="m-0" style="color: red; font-weight: bold">R. D 14, N°113 - JAPIIM -  Fone: (92) 3343-8321</p>
					</div>
				</div>
				<div class="col-md-5 text-center">
					
					<p class="h3 font-weight-bold font-FlamaBold" style="color: #cc0000; text-align: left">Quer saber mais?</p>
					
					<p class="h5 font-FlamaBold" style="color: #696969; text-align: left">Aponte seu celular e conheça o trabalho desta instituição.</p>
					<div  style=" display: flex !important">
					<div style="height: 200px !">
					<img class="img-fluid my-4 " src="static/img/coracao-do-pai-qr-code.jpg" alt="ABRIGO O CORAÇÃO DO PAI">
					</div>
						<div @click.prevent="doar(2)" style="background: #cc0000; width: 180px; height: 110px; margin-left:10px; margin-top: 40px; cursor: pointer;" >
					<a href="" 
                        
                        class=" font-weight-bold    w-70  text-white" style=" font-size:35px;  !important; bottom: 5px !iportant; line-height: 50px;">QUERO DOAR! </a>
					</div>
					</div>
				</div>
			</div>
		</div>
		<!-- -->
		<div class="container pb-1" style="border: 1px solid red !important; margin-bottom:5px; ">
			<div class="row">
				<div class="col-md-6">
					<img class="img-fluid w-100" src="static/img/la-das-maria.jpg" alt="ABRIGO O CORAÇÃO DO PAI">
					<div class="bg-info text-white py-2 px-4" style="background: #ffcc00 !important">
						<h2 class="h4 m-0 font-weight-bold font-FlamaBold" style="color: #2F2F2F">LAR DAS MARIAS</h2>
						<h2 class="h5 m-0 font-weight-bold font-FlamaBold" style="color: #2F2F2F; text-align: justify;">Abriga mulheres em busca de tratamento contra o câncer.</h2>
						<p class="m-0" style="color: red; font-weight: bold">Av. DOM Pedro I, N°984  -  Fone: (92)3307-5337</p>
					</div>
				</div>
				<div class="col-md-5 text-center">
					<p class="h3 font-weight-bold font-FlamaBold" style="color: #cc0000; text-align: left">Quer saber mais?</p>
					<p class="h5 font-FlamaBold" style="color: #696969; text-align: left">Aponte seu celular e conheça o trabalho desta instituição.</p>
					<div  style=" display: flex !important">
						<div>
					<img class="img-fluid my-4" src="static/img/la-das-maria-qr-code.jpg" alt="ABRIGO O CORAÇÃO DO PAI">
						</div>
					<div @click.prevent="doar(3)" style="background: #cc0000; width: 180px; height: 110px; margin-left:10px; margin-top: 40px; cursor: pointer;" >
					<a href="" 
                        
                        class=" font-weight-bold    w-70  text-white" style=" font-size:35px;  !important; bottom: 5px !iportant; line-height: 50px;">QUERO DOAR! </a>
					</div>
				</div>
				</div>
			</div>
		</div>
		<!-- -->
		<div class="container pb-1" style="border: 1px solid red !important; margin-bottom:5px; ">
			<div class="row">
				<div class="col-md-6">
					<img class="img-fluid w-100" src="static/img/abraigo-nacer.jpg" alt="ABRIGO O CORAÇÃO DO PAI">
					<div class="bg-info text-white py-2 px-4 " style="background: #ffcc00 !important">
						<h2 class="h4 m-0 font-weight-bold font-FlamaBold" style="color: #2F2F2F">ABRIGO NACER</h2>
						<h2 class="h5 m-0 font-weight-bold font-FlamaBold" style="color: #2F2F2F; text-align: justify;">Atende crianças e adolescentes em situação de vulnerabilidade</h2>
						<p class="m-0" style="color: red; font-weight: bold">Rua 35, N° 28, CONJUNTO CASTELO BRANCO - PARQUE DEZ - Fone: (92)98428-7454</p>
					</div>
				</div>
				<div class="col-md-5 text-center">
					<p class="h3 font-weight-bold font-FlamaBold" style="color: #cc0000; text-align: left">Quer saber mais?</p>
					<p class="h5 font-FlamaBold" style="color: #696969; text-align: left">Aponte seu celular e conheça o trabalho desta instituição.</p>
					<div  style=" display: flex !important; margin-left: -10px">
						<div>
					<img class="img-fluid my-4" src="static/img/nacer-qr-code.png" alt="ABRIGO O CORAÇÃO DO PAI">
					</div>
					<div  @click.prevent="doar(4)" style="background: #cc0000; width: 180px; height: 110px; margin-left:0px; margin-top: 50px; cursor: pointer;" >
					<a href="" 
                       
                        class=" font-weight-bold    w-70  text-white" style=" font-size:35px;  !important; bottom: 5px !iportant; line-height: 50px;">QUERO DOAR! </a>
					</div>
				</div>
				</div>
			</div>
		</div>

	</div>





        
        <!-- -->
        
        <!-- -->
        
        <!-- -->
        
        
        <div class="vld-parent">
            <loading
                :active.sync="isLoading"
                :can-cancel="false"
                :is-full-page="fullPage"
            ></loading>
            
            
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
    name: 'HelloWorld',
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
            // console.log('asd', idInstitute);
            this.doVote(idInstitute);
        },
        async doVote(idInstitute) {
			this.isLoading = true;
            await axios
                .post(
					'https://api-atack.samel.com.br/institute/vote', // host
					// 'http://192.168.6.250:3000/institute/vote', // host
                    qs.stringify({ institute: idInstitute }), // dados
                    {
                        headers: {
                            'Content-Type': 'application/x-www-form-urlencoded',
                        },
                    }
                )
                .then( async (result) => {
					
					
					if (result.data){
						let thanks = await this.loadThanks(idInstitute)

						let randomNumber = Math.floor(Math.random() * 4) + 1

						// console.log("BBBB", randomNumber - 1)

						let agradecimento = thanks[randomNumber - 1].DS_AGRADECIMENTO.split(" ").join("$")
						

						let nome = thanks[randomNumber - 1].NM_PESSOA_AGRADECIMENTO.split(" ").join("$")

						let nameInstitute = thanks[randomNumber - 1].DS_UNIDADE.split(" ").join("$")
							// console.log("AAA", nome)
							// console.log("BB",thanks[randomNumber - 1].nameInstitute)

						location.href = `http://192.168.6.251:8080/?ds_senha=${agradecimento}&nm_nome=${nome}&nm_institute=${nameInstitute.replace(/ /g, '$' )} `;
						// this.$router.push(`agradecer/?ds_senha=${thanks.DS_AGRADECIMENTO.replace(/ /g, '$')}&nm_nome=${thanks.NM_PESSOA_AGRADECIMENTO}&nm_institute=${this.listInstitute[ idInstitute - 1 ].replace(/ /g, '$' )}`)
					}
					return  result
					
				})
				.finally(() => {
					this.isLoading = false
				})
                .catch((err) => {
                    console.log('Erro ao registar o voto.', err);
                });
        },
        loadThanks(idInstitute) {
			return axios.get(`https://api-atack.samel.com.br/thanks/${idInstitute}`)
			.then((res) => {
                if ( res.data )  {
					return res.data
				}
            });
        },
    },
};


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.page {
	position: absolute;
	left: 50%;
	transform: translateX(-50%);
	background-image: url(../assets/background.jpg);
	 background-size: 1080px 1960px;
	background-repeat: no-repeat, repeat;
	/* width: 100% !important; */
	width: 1080px;
	
	justify-content: center;
	align-items: center;
	margin-bottom: 40px;
}
.pb-5 {
	position: relative;
	width: 89%;
	margin-top: 520px;
	justify-content: center;
	align-items: center;
	margin-left: 58px !important;
	padding: 0px !important;
	margin-bottom: 60px;
	
	
}

h1,
h2 {
    font-weight: normal;
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: inline-block;
    margin: 0 10px;
}
a {
    color: #42b983;
}
.imageWide {
    height: 345px;
    object-fit: cover;
	
}
</style>
