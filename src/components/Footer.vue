<template>
        <footer class="footer">
            <div class="container">
                <div class="footer-box">
                    <router-link to="/" class="footer-logo logo">
                        <img src="../assets/images/logo.png" alt="logo">
                    </router-link>
                    <div class="footer-nav">
                        <ul>
                            <li>Ресторанам </li>
                            <li>Курьерам</li>
                            <li>Пресс-центр</li>
                            <li>Контакты</li>
                        </ul>
                    </div>
                    <div class="footer-social">
                        <img src="../assets/images/social/instagram.svg" alt="instagram">
                        <img src="../assets/images/social/facebook.svg" alt="facebook">
                        <img src="../assets/images/social/vk.svg" alt="vk">
                    </div>
                </div>
            </div>
        </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
.footer {
    display: flex;
    align-items: center;
    min-height: 156px;
    padding: 60px 0;
}

.footer-box {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 36px;
}

.footer-nav {
    flex-grow: 1;
}

.footer-nav ul {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    list-style: none;
    padding: 0;
    margin: 0;
    gap: 15px;
}

.footer-nav ul li {
    font-size: 18px;
    font-weight: 400;
    color:#595959;
}

.footer-social {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    gap: 20px;
}
</style>