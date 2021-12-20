<template>
  <div>


<div class="header">
  <h2>Aprendendo Vue</h2>
</div>

  <div class="row">
    <div class="column" style="background-color:#aaa;">   <life-cycle />
  </div>
    <div class="column" style="background-color:#bbb;">    <teste-component/>
  </div>
    <div class="column" style="background-color:#ccc;">    <pessoa />
  </div>
  </div>

<div class="footer">
  <p>Footer</p>
</div>

   
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

<style>
* {
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}

/* Style the header */
.header {
  background-color: #f1f1f1;
  padding: 30px;
  text-align: center;
  font-size: 35px;
}

/* Create three equal columns that floats next to each other */
.column {
  float: left;
  width: 33.33%;
  padding: 10px;
  height: 300px; /* Should be removed. Only for demonstration */
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Style the footer */
.footer {
  background-color: #f1f1f1;
  padding: 10px;
  text-align: center;
}

/* Responsive layout - makes the three columns stack on top of each other instead of next to each other */
@media (max-width: 600px) {
  .column {
    width: 100%;
  }
}
</style>