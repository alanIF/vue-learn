<template>
    <div>
        <ul>
            <li>{{nome}}</li>
            <li>{{profissao}}</li>
            <li>{{email}}</li>
        </ul>
    </div>
</template>

<script>
    export default{
        name:"Pessoa",
        
        data(){
            return{
                nome:"Alan",
                profissao:"programador"
            }
        }
        
    }
</script>
