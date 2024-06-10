<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="bg">
        <div class="container">
            <button>sign-up now!</button>
            <nav class="flex-centered">
                <h3>follow us</h3>
                <section>
                    <a href=""><img src="../assets/img/footer-facebook.png" alt=""></a>
                    <a href=""><img src="../assets/img/footer-twitter.png" alt=""></a>
                    <a href=""><img src="../assets/img/footer-youtube.png" alt=""></a>
                    <a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a>
                    <a href=""><img src="../assets/img/footer-periscope.png" alt=""></a>
                </section>
            </nav>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

div.bg {
    background-color: $dc-gray;
    div{
        width: 100%;
        display: flex;
        justify-content: space-between;
        padding: 2rem 0;
        
        h3 {
            color: $dc-blue;
            text-transform: uppercase;
            margin-right: 1.5rem;
            font-size: 1.4rem;
        }

        a {
            margin-right: 1rem;
        }
    }

    button {
        border: 2px solid $dc-blue;
        background-color: transparent;
        font-family: "Roboto", sans-serif;
        font-weight: bold;
        font-size: 1.2rem;
        color: white;
        text-transform: uppercase;
        padding: .8rem;
    }
}


</style>