<template>
    <div class="card">

        <h1>{{card_name}} </h1>
        <p class="email">{{card_email}}</p>

    </div>
</template>

<script>
    export default {
        props: {
            card_name: {
                type: String
            },
            card_email: {
                type: String
            }
        },
        
    }
</script>

<style>
.card{
    padding-right: 20px;
    height: 373px;
    border-radius: 2px;
    display: flex;
    flex-direction: column;
    justify-content: start;
        padding-right: 20px;
    padding-left: 20px;
}
.card .email{
    font-size: 18px;
    width: 80%;
    background-color: teal;
    float: right;
    text-align: center;
}

</style>