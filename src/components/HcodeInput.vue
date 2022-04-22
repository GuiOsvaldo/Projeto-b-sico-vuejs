<template>
    <input type="text" :value="value" @keyup="$emit('input' , $event.target.value)" 
    placeholder="Digite o seu clube" class="form-control">
</template>

<script>

export default{
   props:{
       value: String
   }
}
</script>
<style scoped>

</style>