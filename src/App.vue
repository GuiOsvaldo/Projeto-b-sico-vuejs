<template>
<div class  id="app">  
  <HcodeHeader @select-championship="changeChampionship" />
  <HcodeSection :championship="championship" />
   <HcodeFooter/>
 </div>
 </template>

<script>

import HcodeHeader from './components/HcodeHeader'
import HcodeFooter from './components/HcodeFooter'
import HcodeSection from './components/HcodeSection'

export default {
  name: 'App',
  components: {
     HcodeHeader,
     HcodeFooter,
     HcodeSection
  },
    data(){
      return{
        championship: 'Campeonato Brasileiro'
      }
    },
    methods: {
      changeChampionship(value){
             this.championship = value;
      }
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Rajdhani&display=swap')
</style>
