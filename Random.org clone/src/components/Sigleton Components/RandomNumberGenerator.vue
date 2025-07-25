<template>
    <div class="container">
        <div class="small-title">
            True Random Number 
            Generator
        </div>
        <div class="min-container">
            Min: 
            <input type="number" v-model="min">
        </div>
        <div class="max-container">
            Max: 
            <input type="number" v-model="max">
        </div>
        <button type="button" @click="generateRandomNumber">Generate</button>
        <div class="result-container">
            Result:
            <div class="result">{{ result }}</div>
        </div>
    </div>
</template>

<script>
    export default{
        data(){
            return {
                min: 1,
                max: 100,
                result: null
            }
        },
        methods:{
            generateRandomNumber(){
                this.result = Math.floor(Math.random() * (this.max+1 - this.min) + this.min);
            }
        }
    }
</script>

<style scoped>
    .container{
        border: 1px solid #CCCCFF;
        height: 180px;
        width: 160px;

        display: flex;
        flex-direction: column;
        gap: 4px;

        div{
            margin: 0 5px;
            &:first-child{
                margin: 0;
            }

            align-items: center;

            font-size: 12px;
            color: #777;

            input{
                width: 84px;
                font-size: 0.82rem;
            }
        }
        div.min-container{
            input{
                margin: 0 3px
            }
        }

        .min-container{
            gap: 13.5px;
            margin-top: 4px;
        }

        button{
            margin: 4px;
            width: 71px;
        }

        .result-container{

            .result{
                padding: 7px 0;
                background-color: #CCCCFF;
                color: black;
                text-align: center;
                font-size: 1.4rem;
                height:max-content
            }
        }
    }

    .small-title{
        font-size: 13px;
        text-align: center;
        background-color: #CCCCFF;
    }

</style>