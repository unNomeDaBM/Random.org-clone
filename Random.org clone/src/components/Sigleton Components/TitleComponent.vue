<template>
    <div class="title-container">
        <img src="../Assets/main_title.png" alt="" width="60%">
        <div class="search-bar">
            <span class="mini-sub-title">Search RANDOM.ORG</span><br>
            <input type="text" name="q" size="16">
            <input type="submit" value="Search"><br>
            <span class="sub-title">True Random Number Service</span>
        </div>
    </div>
</template>

<script>

</script>

<style scoped>
    .title-container{
        display: flex;
        justify-content: space-between;
    }
    .search-bar{
        text-align: end;
    }
    .mini-sub-title{
        font-size: 0.65rem;
        margin: 0 95px 0 0
    }
    input{
        margin: 0 3px 0 0;
    }
    .sub-title{
        position: relative;
        top: 10px;
        left: -4px;
        font-size: 0.95rem;
        font-weight: 700;
    }
</style>