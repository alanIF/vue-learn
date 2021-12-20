<template>
  <div>
    <h1>Teste</h1>
    <life-cycle />
    <teste-component/>
    </div>
</template>

<script>

  import TesteComponent from './components/TesteComponent.vue';
  import LifeCycle from './components/LifeCycle.vue';
  export default{
    name:'app',
    components:{
      TesteComponent,
      LifeCycle
    }
  }
</script>
