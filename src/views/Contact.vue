<template>
    <div class="body">
        <div class="body-details">
            <div class="body-details-header">
                <h1>Contact</h1>
            </div>
            <div class="body-details-body">
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt vitae placeat expedita saepe aut incidunt voluptates non ipsa iusto, eum aperiam in molestiae cupiditate
                    doloremque ducimus recusandae adipisci possimus unde ratione labore esse atque eos vero. Iure tempora dicta beatae et quibusdam in. Consequuntur iure corporis quia exercitationem
                    totam laborum, magni qui ducimus excepturi labore commodi harum culpa aperiam sint maiores similique, numquam voluptatem, alias quos! Deleniti dolor numquam et.
                </p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Home',
        components: {},
        props: {}
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .body {
        width: 100%;
        display: flex;
        justify-content: center;
        margin-top: 50px;
    }
    .body-details {
        width: 45%;
    }
    .body-details-header h1 {
        font-size: 4rem;
        text-align: start;
        margin-bottom: 50px;
    }
    .body-details-body {
        margin-bottom: 100px;
    }
    .body-details-body p {
        text-align: start;
    }
    h1 {
        color: black;
    }
</style>
