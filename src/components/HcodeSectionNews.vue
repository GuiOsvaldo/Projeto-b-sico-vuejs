<template>
    <section>
        <div class="container">  

        <HcodeSectionNewsIndividual 
        img-name="news1.jpg"
        img-info="Notícia 1"
        news-title="Começam os treinos para a nova temporada"
        news-content="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Neque eligendi ipsum nobis veniam quidem necessitatibus quis magni, error inventore vitae vel. 
        Repudiandae maiores quisquam, esse harum sapiente odit error blanditiis!                    
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci molestias placeat perferendis quas, numquam praesentium eveniet laborum eius vitae ullam magnam consequatur.
        Facilis praesentium itaque illum placeat dicta. Maxime, voluptatem."
        news-date="02/12/2013"
        />
        <HcodeSectionNewsIndividual 
        img-name="news2.jpg"
        img-info="Notícia 2"
        news-title="Próximas competições"
        news-content="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Neque eligendi ipsum nobis veniam quidem necessitatibus quis magni, error inventore vitae vel. 
        Repudiandae maiores quisquam, esse harum sapiente odit error blanditiis!                    
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci molestias placeat perferendis quas, numquam praesentium eveniet laborum eius vitae ullam magnam consequatur.
        Facilis praesentium itaque illum placeat dicta. Maxime, voluptatem."
        news-date="02/02/2017"
        
        />

<HcodeSectionNewsIndividual 

        img-name="news3.jpg"
        img-info="Notícia 3"
        news-title="Jogos Extras"
        news-content="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Neque eligendi ipsum nobis veniam quidem necessitatibus quis magni, error inventore vitae vel. 
        Repudiandae maiores quisquam, esse harum sapiente odit error blanditiis!                    
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci molestias placeat perferendis quas, numquam praesentium eveniet laborum eius vitae ullam magnam consequatur.
        Facilis praesentium itaque illum placeat dicta. Maxime, voluptatem."
        news-date="12/10/2021"

/>
    </div>
        </section>
</template>

<script>
 import HcodeSectionNewsIndividual from './HcodeSectionNewsIndividual'
export default {
      components: {
          HcodeSectionNewsIndividual
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