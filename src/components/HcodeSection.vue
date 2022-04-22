<template>
 
     <div class="container">
           <div class="row mt-5">
            <h5> Você está vendo nótícias do: {{ championship }} </h5>
           </div>
     </div>
<div >
     
      
  <component :is="currentComponent"></component>
     
      
         
        
       
        <div class="container">

 <div class="row my-club mt-5">
    
      <div class="col-6">
          <h2> Seu Clube é: {{ myClub }} </h2>
      </div>
      <div class="col-6">
           <HcodeInput v-model="myClub"/>
      </div>

     </div>
     </div>
    </div>
</template>

<script>
 import HcodeSectionBanner from './HcodeSectionBanner' 
 import HcodeSectionNews from './HcodeSectionNews' 
 import HcodeInput from './HcodeInput'


export default {
    components:{
        HcodeSectionBanner,
        HcodeSectionNews,
        HcodeInput
       
    },
    data(){
        return {
            myClub: 'Hcode Treinamentos',
            
        }
    },
      props:{
          championship: String,
           currentComponent: String
      }
}
</script>

<style scoped>
section{
    padding:50px 0;
    margin-top:25px;
    background-color:#f37520;
}
</style>
