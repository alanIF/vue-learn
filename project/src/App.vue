<template>
  <div>
    <h1>Teste</h1>
    <life-cycle />
    <teste-component/>
    <pessoa />
    </div>
</template>

<script>

  import TesteComponent from './components/TesteComponent.vue';
  import LifeCycle from './components/LifeCycle.vue';
  import Pessoa from './components/Pessoa.vue';

  export default{
    name:'app',
    components:{
      TesteComponent,
      LifeCycle,
        Pessoa
    }
  }
</script>
