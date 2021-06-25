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
}
.card .email{
    font-size: 38px;
    margin-right: 20px;
    margin-left: 20px;
}

</style>