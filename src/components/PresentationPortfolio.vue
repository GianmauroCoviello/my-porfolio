
<script>
export default {
    name: 'PresentationPortfolio',

    data() {
        return {
            IconComp: [
                {
                    label: 'HTML',
                    link: 'https://img2.gratispng.com/20180802/tpl/kisspng-logo-html5-brand-clip-art-%E6%9D%89-%E5%B1%B1-%E8%89%AF-%E9%9B%84-5b62be01b565d5.334247781533197825743.jpg'
                    
                },
                {
                    label: 'CSS',
                    link: 'https://clipartcraft.com/images/html5-logo-transparent-4.png'
                    
                },
                {
                    label: 'JAVASCRIPT',
                    link:'https://tse2.mm.bing.net/th?id=OIP.9OYrZr6Hw8jJXgOM6tAI4QHaIY&pid=Api&P=0&h=180'
                    
                },
                {
                    label: 'SASS',
                    link:'https://tse3.mm.bing.net/th?id=OIP.bUVK5EiCXfTNgPt2vQu9agHaHa&pid=Api&P=0&h=180'
                    
                },
                {
                    label: 'BOOTSTRAP',
                    link:'http://getbootstrap.com/docs/3.3/assets/brand/bootstrap-solid.svg'
                    
                },
                {
                    label: 'PHP',
                    link:'https://logos-download.com/wp-content/uploads/2016/09/PHP_logo.png'
                    
                },
                {
                    label: 'MYSQL',
                    link:'https://www.geekandjob.com/uploads/wiki/eceb15684d4183c66f73c1a9bb777eef708b2b66.png'
                    
                },
                {
                    label: 'VUE',
                    link:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTGOkHT-Um9X2PkngU4jpLZhXwZ0GgsZasuKA&usqp=CAU'
                    
                },
                {
                    label: 'LARAVEL',
                    link:'https://res.cloudinary.com/teepublic/image/private/s--otbkTXps--/c_crop,x_10,y_10/c_fit,w_841/c_crop,g_north_west,h_1038,w_1038,x_-97,y_-396/l_upload:v1565806151:production:blanks:vdbwo35fw6qtflw9kezw/fl_layer_apply,g_north_west,x_-208,y_-507/b_rgb:000000/c_limit,f_auto,h_630,q_auto:good:420,w_630/v1654831631/production/designs/31437719_0.jpg'
                    
                },
     

            ]
        }
    },

}
</script>
<template>
    <header>
        <div class="container">
            <div class="row ">
                <div class="col-12 mb-5">
                    <h1 class="text-center mt-4 text-primary parti" ><em>Hi, I'm Gianmauro Coviello</em></h1>
                    <h3 class="text-center mt-4 text-primary parti" >{<em> Full Stack Web Developer   </em>}</h3>
                </div>
                <div class="squares row">
                    <div class="col-5 ps-5 mt-3">
                        <img class="rounded-circle" src="https://media.licdn.com/dms/image/D4D03AQFLnBXL2YSHBQ/profile-displayphoto-shrink_400_400/0/1694191277566?e=1703721600&v=beta&t=5ylQZEbNswgjIynTxRmQFhq-ML_MjxuVnY6gfQLpwAw" alt="">
                    </div>
                    <div class="col-7 mt-3">
                        <h5 class="text-primary">PROFILO PERSONALE:</h5>
                        <p class="text-light"><em>Sono un ragazzo con molta voglia di fare ed imparare. Sicuramente sono una persona molto ambiziosa e curiosa nell'imparare ed interagire con le nuove tecnologie e linguaggi che nel mondo della programmazione sono in continua evoluzione. Sempre pronto ad intraprendere nuove sfide.</em></p>
                        <h5 class="text-primary">COMPETENZE PERSONALI</h5>
                        <ul class="text-light ps-0">
                            <li>Capacità di problem solving</li>
                            <li>Gestione ed organizzazione del lavoro in maniera precisa</li>
                            <li>Puntualità e massima serietà</li>
                            <li>Molta voglia di imparare ed incrementare le mie competenze</li>
                            <li>Ottime capacità di comunicazione</li>
                            

                        </ul>
                        <h5 class="text-primary">CONTATTI</h5>
                        <ul class="text-light ps-0">
                            <li>
                                <i class="fa-solid fa-beat text-light pe-3 pb-3 fa-envelope "></i>
                                <span>gianmaurocoviello@gmail.com</span>
                            </li>
                            <li>
                                <i class="fa-solid fa-shake text-primary pe-3 pb-3 fa-phone "></i>
                                <span>+39 371 320 2672</span>
                            </li>
                            <li>
                                <i class="fa-solid fa-bounce text-danger pe-3 pb-3 fa-house "></i>
                                <span>Bari 70100</span>
                            </li>
                            
                        </ul>
                    </div>
                </div>
                
                <div class="col-12">
                    <h5 class="text-primary my-5 text-center">LE MIE COMPETENZE:</h5>
                    <ul class="d-flex flex-wrap justify-content-center">

                        <li class="" v-for="(item, index) in IconComp" :key="index">
                            <!-- <h1 class="text-light">{{ item.label }}</h1> -->
                            <div class="container-competence text-center">
                                <img class="pb-1" :src="`${item.link}`" alt="">
                                <p class="text-center text-light "><em>{{ item.label }}</em></p>
                            </div>
                            
                        </li>
                        
                        
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>


<style lang="scss" scoped>
ul{
    list-style-type: none;

    img{
        width: 80px;
        height: 80px;
        border-radius: 50%;

        &:hover{
            width: 120px;
            height: 120px;
            transition: 1.5s;


        }
        
    }

    .container-competence{
        width: 160px;
        height: 160px;
    }

    
    
}

.squares{
        border-radius: 20px;
        background-color: rgba(76, 78, 98, 0.546);
        padding-bottom: 40px;
        padding-top: 20px;
        // opacity: 60%;
}


    
</style>