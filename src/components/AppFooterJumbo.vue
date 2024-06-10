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
            <nav>
                <p>follow us</p>
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
}
</style>