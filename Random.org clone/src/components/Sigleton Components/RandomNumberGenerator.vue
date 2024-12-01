<template>
    <div class="container">
        <div class="small-title">
            True Random Number 
            Generator
        </div>
        <div class="min-container">
            Min: 
            <input type="number" name="" id="">
        </div>
        <div class="max-container">
            Max: 
            <input type="number" name="" id="">
        </div>
        <button type="button">Generate</button>
        <div class="result-container">
            Result:
            <div class="result">12</div>
        </div>
    </div>
</template>

<script>
    export default{
        
    }
</script>

<style scoped>
    .container{
        border: 1px solid #CCCCFF;
        height: 160px;
        width: 160px;

        display: flex;
        flex-direction: column;
        gap: 4px;

        div{
            margin: 0 5px;
            &:first-child{
                margin: 0;
            }

            display: flex;
            flex-direction: row;
            align-items: center;
            gap: 10px;

            font-size: 12px;
            color: #777;

            input{
                width: 84px;
                font-size: 0.82rem;
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

        .result-cotainer{
            display: block;

            .result{
                background-color: #CCCCFF;
                height: 4px;
            }
        }
    }

    .small-title{
        font-size: 13px;
        text-align: center;
        background-color: #CCCCFF;
    }

</style>