<template>
    <div>
        <h1>Primeiro Componente</h1>
        <p>{{nome}}</p>
    </div>
</template>

<script>

export default {
   name:"PrimeiroComponente" ,
   data(){
       return{
           nome:"Alan"
       }
   }
}
</script>
