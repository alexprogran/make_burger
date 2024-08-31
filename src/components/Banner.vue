<template>
    <div id="main-banner">
        <h1>Make Your Burger</h1>

    </div>
</template>

<script>
export default{
name:"Banner",
}
</script>

<style scoped>
#main-banner{
    background-image: url('/public/img/burger.jpg');
    background-position: 0 -320px;
    background-size: cover;
    height:525px;
    display: flex;
    align-items: center;
    Justify-content: flex-start;
}

#main-banner h1{
    color: #DDD;
    text-align: center;
    font-size: 40px;
    background-color: #222;
    padding: 20px 40px;
}

</style>
