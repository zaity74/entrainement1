<template>
    <div class="card">

        <h1>{{card_name}} </h1>
        <p>{{card_email}}</p>

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
    height: 373px;
    border-radius: 2px;
}

</style>