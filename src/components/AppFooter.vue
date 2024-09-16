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
        <div class="container">
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
        </div>
        <!--sign-up and socials-->
        <section id="footer-info">
            <div class="container">
                <div class="footer-link">
                    <!--Sign-up-->
                    <div id="sign">ciao</div>
                    <!--Socials-->
                    <div id="socials">
                        <h3>FOLLOW US</h3>
                        <ul>
                            <li><a href="#">social</a></li>
                            <li><a href="#">social</a></li>
                            <li><a href="#">social</a></li>
                            <li><a href="#">social</a></li>
                            <li><a href="#">social</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
footer {
    padding: 40px 0;
    background-color: green;
    height: 450px;

    #general-links {
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
            }

            li {
                margin-bottom: 5px;
            }
        }
    }

    /*Socials*/
    #footer-info {
        background-color: gray;
        height: 80px;

        .footer-link {
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        #socials {
            display: flex;
            gap: 25px;

            ul {
                display: flex;
                gap: 15px;
            }
        }
    }
}
</style>
