<template>
    <div class="container">
        <h1>Count</h1>
        <div class="count-btn">
            <button @click="count++">Count is: {{ count }}</button>
            <button @click="count=0">Reset</button>
        </div>
        <div class="count-btn count-btn-2">
            <span>{{ count2 }}</span>
            <button @click="count2+=1">Increment</button>
            <button @click="count2-=1">Decrement</button>
            <button @click="count2=0">Reset</button>
        </div>
    </div>
</template>

<script>
    export default{
        name: 'CountApp',
        data(){
            return{
                count: 0,
                count2: 0
            }
        }
    }
</script>

<style scoped>
    .container{
        display: flex;
        flex-flow: column wrap;
        margin-top: -4%;
    }

    .container h1{
        font-size: 35pt;
    }

    .count-btn{
        margin-top: 5%;
    }

    .count-btn button{
        padding: 1rem;
        width: 10rem;
        margin-left: 2%;
        cursor: pointer;
        border-radius: 6px;
        font-size: 14pt;
    }

    .count-btn-2{
        margin-top: 2%;
    }

    .count-btn-2 span{
        display: block;
        font-size: 50pt;
    }

    .count-btn-2 button{
        margin-top: 4%;
        margin-left: 2%;
    }
</style>