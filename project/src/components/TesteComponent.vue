<template>
    <div>
        <h1>Testes de Diretivas</h1>
        <p v-if="exibir">{{nome}}</p>
        <p v-else>Nao é verdadeiro</p>
        <a v-bind:href="link" target="_blank">google</a>
        <button @click="show">Alerta</button>
    </div>
</template>

<script>

export default {
   name:"PrimeiroComponente" ,
   data(){
       return{
           nome:"Alan Tavares",
           exibir:false,
           link: "https://google.com"
       }
      
   },
    methods:{
        show(){
            this.exibir= true;
            alert("Ola metodo")
        }
    }
}
</script>
