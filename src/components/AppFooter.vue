<script>
export default {
    data() {
        return {
            dcComics: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],
            shop: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            dc: [
                "Terms Of Use",
                "Privacy policy (New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshop",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contacts Us"
            ],
            sites: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ]
        }
    }
}
</script>

<template>
    <footer>
        <div id="footer-top" class="container">
            <!--General Links-->
            <nav id="general-links">
                <div class="dc-comics">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li v-for="link in dcComics"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
                <div class="shop">
                    <h3>SHOP</h3>
                    <ul>
                        <li v-for="link in shop"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
                <div class="dc">
                    <h3>DC</h3>
                    <ul>
                        <li v-for="link in dc"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
                <div class="sites">
                    <h3>SITES</h3>
                    <ul>
                        <li v-for="link in sites"><a href="#">{{ link }}</a></li>
                    </ul>
                </div>
            </nav>
            <div id="logo-bg"></div>
        </div>
        <!--sign-up and socials-->
        <section id="footer-info">
            <div class="container">
                <div class="footer-link">
                    <!--Sign-up-->
                    <div id="sign"><button>SIGN-UP NOW!</button></div>
                    <!--Socials-->
                    <div id="socials">
                        <h3>FOLLOW US</h3>
                        <ul>
                            <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="YouTube"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a></li>
                            <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="Maps"></a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 400px;

    #footer-top {
        display: flex;
        justify-content: space-between;
    }

    #logo-bg {
        height: 500px;
        width: 600px;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        position: relative;
        bottom: 80px;
    }

    #general-links {
        padding-top: 50px;
        height: 100%;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        width: fit-content;

        .dc-comics,
        .shop,
        .dc,
        .sites {
            margin-right: 30px;
            margin-bottom: 20px;

            h3 {
                margin-bottom: 15px;
                color: white;
            }

            li {
                margin-bottom: 7px;

                a {
                    color: gray;
                }
            }
        }
    }

    /*Socials*/
    #footer-info {
        background-color: #303030;
        height: 80px;
        position: relative;
        z-index: 1;

        .footer-link {
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: space-between;

            button {
                padding: 10px 15px;
                background-color: #303030;
                border: 2px solid #0282F9;
                color: white;
                cursor: pointer;
            }
        }

        #socials {
            display: flex;
            align-items: center;
            gap: 25px;
            color: #0282F9;
            height: 100%;

            ul {
                display: flex;
                gap: 15px;
            }
        }
    }
}
</style>
