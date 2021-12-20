<template>
    <div>
        <h1>Painel</h1>
        <h2>{{dados}}</h2>
    </div>
</template>

<script>
    export default{
        name:"LifeCycle",
        data(){
            return{
                dados:"1,2,3"
            }
        },
        created(){
            this.dados= "Home"
        }
    }
</script>
