<template>
    <section>
        <div class="container">  

        <HcodeSectionNewsIndividual 
         v-for="notice in news"
         :key="notice.id"
         :img-name="notice.img"
         :img-info="notice.imgInfo"
         :news-title="notice.title"         
         :news-date="notice.date"
        >
              <template #title>
                   <h2> {{notice.title}} </h2>
              </template>
              <p>
               {{ notice.content }}  
                 </p>
        </HcodeSectionNewsIndividual>


    </div>
        </section>
</template>

<script>
 import HcodeSectionNewsIndividual from './HcodeSectionNewsIndividual'
export default {
      components: {
          HcodeSectionNewsIndividual
      },
       data(){
           return{
               news: []
           }
       },
       created(){
           this.news = [{
               id: 1,
               title: 'Começam os treinos para a nova temporada',
               content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Neque eligendi ipsum nobis veniam quidem necessitatibus quis magni, error inventore vitae vel. Repudiandae maiores quisquam, esse harum sapiente odit error blanditiis!                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci molestias placeat perferendis quas,numquam praesentium eveniet laborum eius vitae ullam magnam consequatur.Facilis praesentium itaque illum placeat dicta. Maxime, voluptatem.',
               date: '2013-12-02',
               img: 'news1.jpg',
               imgInfo: 'Notícia 1' 
           },{
                 id: 2,
               title: 'Próximas competições',
               content: ' error inventore vitae vel. Repudiandae maiores quisquam, esse harum sapiente odit error blanditiis!Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci molestias placeat perferendis quas,numquam praesentium eveniet laborum eius vitae ullam magnam consequatur.Facilis praesentium itaque illum placeat dicta. Maxime, voluptatem.',
               date: '2017-02-04',
               img: 'news2.jpg',
               imgInfo: 'Notícia 2' 
           }, {
               id: 3,
               title: 'Jogos Extras',
               content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Neque eligendi ipsum nobis veniam quidem necessitatibus quis magni, error inventore vitae vel. Repudiandae maiores quisquam, esse harum sapiente odit error blanditiis!                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci molestias placeat perferendis quas,numquam praesentium eveniet laborum eius vitae ullam magnam consequatur.Facilis praesentium itaque illum placeat dicta. Maxime, voluptatem.',
               date: '2013-12-02',
               img: 'news3.jpg',
               imgInfo: 'Notícia 3' 
           }]
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