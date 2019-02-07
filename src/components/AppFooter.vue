<template>
    <footer class="footer">
        <div class="footer-contacts">
            <h1>Copyright &copy; Neil Aldrei Peralta</h1>
            <p>neilaldreiii@gmail.com</p>
            <p>+63915-204-4704</p>
        </div>
        <div class="footer-social">
            <a href="https://www.messenger.com/t/dreiiin" target="_blank" class="messenger"><i class="fab fa-facebook-messenger"></i></a>
            <a href="https://github.com/neilaldreiii" target="_blank" class="github"><i class="fab fa-github"></i></a>
            <a href="https://twitter.com/neilaldrei" target="_blank" class="twitter"><i class="fab fa-twitter"></i></a>
        </div>
    </footer>
</template>

<script>
export default {
    name: "footer",
    data() {
        return {

        }
    }
}
</script>

<style scoped>
h1 {
    font-family: 'Open Sans', sans-serif;
    margin: 15px 0;
}
.footer-social {
    display: flex;
    flex-flow: row;
    justify-content: space-evenly;
    width: 30%;
    padding: 20px;
}
.footer-social a {
    font-size: 28pt;
}
</style>
