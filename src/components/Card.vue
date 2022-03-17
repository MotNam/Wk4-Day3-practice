<template>
 
<div>
         
    <div class="title">{{title}}</div>
    <div class="title">{{description}}</div>
 
    <Buton :name='buton' bgColor='Blue' />
</div>

</template>

<script>
import Buton from "./Buton.vue"

export default {
components:{
    Buton,
},
name: 'Card',
    props:{
    title: String,
    description: String,
    button: String
  },

}
</script>

<style scoped>
    .title {
        color: red;
    }
</style>



