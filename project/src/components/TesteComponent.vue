<template>
    <div>
        <h1>Testes de Diretivas</h1>
        <p v-if="exibir">{{nome}}</p>
        <p v-else>Nao é verdadeiro</p>
        <a v-bind:href="link" target="_blank">google</a>
        <button @click="show">Alerta</button>
        <ul >
            <li v-for="(l,index) in lista" v-bind:key="index">{{l}}</li>
        </ul>
          <ul >
            <li v-for="l in lista2" v-bind:key="l.id">{{l.nome}} -{{l.email}}  </li>
        </ul>
        <h3>Recebendo valor externo: {{ teste}}</h3>
    </div>
</template>

<script>

export default {
   name:"PrimeiroComponente" ,
   props:{
    teste:String
   },
   data(){
       return{
           nome:"Alan Tavares",
           exibir:false,
           link: "https://google.com",
           lista: ['Alan', 'Jose', 'Wanessa'],
           lista2:[
               {
                   id:1,
                   nome:"Alan",
                   email:"alan_tj@hotmail.com.br"
               },
               { 
                   id:2,
                   nome:"wANESSA",
                   email:"wanessa@hotmail.com.br"},
               {id:3,
                   nome:"jose",
                   email:"jose@hotmail.com.br"}
           ]
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
