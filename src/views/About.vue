<template>
    <div class="body">
        <div class="body-details">
            <div class="body-details-header">
                <h1>About</h1>
            </div>
            <div class="body-details-body">
                <p>
                    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ipsam quo molestias quis amet repudiandae eos rem aliquid vero earum quam porro magnam, maiores laudantium ad! Fuga
                    temporibus quasi delectus tenetur dolore culpa optio cumque blanditiis consequuntur ab odit praesentium, non deleniti neque id autem amet reprehenderit nobis libero ipsa!
                    Voluptates!
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
