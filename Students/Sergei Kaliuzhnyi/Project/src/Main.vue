<template>
    <div>
        <header class="header center">
            <div class="header__left">
                <a class="logo" href="index.html">
                    <img class="logo__img" src="https://raw.githubusercontent.com/eqillibrium/My_Store_API/master/logo.png" alt="logo">BRAN<span class="accent">D</span>
                </a>
                <form class="header__form" action="#">
                    <div class="browse">Browse <i class="fa fa-sort-desc browse__icon" aria-hidden="true"></i></div>
                    <input type="text" value="Search for Item..." class="input_text">
                    <button class="search_button"><img src="https://raw.githubusercontent.com/eqillibrium/My_Store_API/master/search.png" alt="search"></button>
                </form>
            </div>
            <div class="header__right">
                <button class="header__basket-button" id="basket-toggler" @click="showBasket = !showBasket"><img
                            class="header__cart" src="https://raw.githubusercontent.com/eqillibrium/My_Store_API/master/basket.png" alt="cart"></button>

                <Basket v-show="showBasket" ref="basket"/>
                
                <a href="#" class="button">My Account <i class="fa fa-sort-desc button__icon"
                        aria-hidden="true"></i></a>
            </div>
        </header>
        <header class="nav">
            <ul class="menu center">
                <li class="menu__list"><a href="index.html" class="menu__link">Home</a></li>
                <li class="menu__list">
                    <a href="product.html" class="menu__link">Man</a>
                    <div class="drop">
                        <div class="drop__flex">
                            <h3 class="drop__h3">Women</h3>
                            <ul class="drop__ul">
                                <li><a href="product.html" class="drop__a">Dresses </a></li>
                                <li><a href="product.html" class="drop__a">Blazers </a></li>
                                <li><a href="product.html" class="drop__a">Denim </a></li>
                                <li><a href="product.html" class="drop__a">Leggings/Pants </a></li>
                                <li><a href="product.html" class="drop__a">Skirts/Shorts </a></li>
                                <li><a href="product.html" class="drop__a">Accessories</a></li>
                            </ul>
                        </div>
                        <div class="drop__flex">
                            <h3 class="drop__h3">Women</h3>
                            <ul class="drop__ul">
                                <li><a href="product.html" class="drop__a">Dresses </a></li>
                                <li><a href="product.html" class="drop__a">Tops </a></li>
                                <li><a href="product.html" class="drop__a">Sweaters/Knits </a></li>
                            </ul>
                        </div>
                    </div>
                </li>
                <li class="menu__list"><a href="single_page.html" class="menu__link">Women</a></li>
                <li class="menu__list"><a href="product.html" class="menu__link">Kids</a></li>
                <li class="menu__list"><a href="product.html" class="menu__link">Accoseriese</a></li>
                <li class="menu__list"><a href="product.html" class="menu__link">Featured</a></li>
                <li class="menu__list"><a href="product.html" class="menu__link">Hot Deals</a>
                    <div class="drop drop_last">
                        <div class="drop__flex">
                            <h3 class="drop__h3">Women</h3>
                            <ul class="drop__ul">
                                <li><a href="product.html" class="drop__a">Dresses </a></li>
                                <li><a href="product.html" class="drop__a">Blazers </a></li>
                                <li><a href="product.html" class="drop__a">Denim </a></li>
                                <li><a href="product.html" class="drop__a">Leggings/Pants </a></li>
                                <li><a href="product.html" class="drop__a">Skirts/Shorts </a></li>
                                <li><a href="product.html" class="drop__a">Accessories</a></li>
                            </ul>
                        </div>
                        <div class="drop__flex">
                            <h3 class="drop__h3">Women</h3>
                            <ul class="drop__ul">
                                <li><a href="product.html" class="drop__a">Dresses </a></li>
                                <li><a href="product.html" class="drop__a">Tops </a></li>
                                <li><a href="product.html" class="drop__a">Sweaters/Knits </a></li>
                            </ul>
                        </div>
                    </div>
                </li>
            </ul>
        </header>
        <!-- <div class="promo">
        <div class="center promo__box">
            <div class="promo__content">
                <h1 class="promo__h1">THE BRAND</h1>
                <h2 class="promo__h2">OF LUXERIOUS FASHION</h2>
            </div>
        </div>
    </div>
    <section class="offers center">
        <div class="offers__left">
            <a href="product.html">
                <div class="offers__content-one">
                    <div class="offers__text">
                        <h2 class="offers__content-h2">hot deal</h2>
                        <h2 class="offers__content-h1">for men</h2>
                    </div>
                </div>
            </a>
            <a href="product.html">
                <div class="offers__content-three">
                    <div class="offers__text">
                        <h2 class="offers__content-h2">30% offer</h2>
                        <h2 class="offers__content-h1">women</h2>
                    </div>
                </div>
            </a>
        </div>
        <div class="offers_right">
            <a href="product.html">
                <div class="offers__content-two">
                    <div class="offers__text">
                        <h2 class="offers__content-h2">LUXIROUS & trendy</h2>
                        <h2 class="offers__content-h1">ACCESORIES</h2>
                    </div>
                </div>
            </a>
            <a href="product.html">
                <div class="offers__content-four">
                    <div class="offers__text">
                        <h2 class="offers__content-h2">new arrivals</h2>
                        <h2 class="offers__content-h1">FOR kids</h2>
                    </div>
                </div>
            </a>
        </div>
    </section> -->
        <section class="featured center">
            <div class="featured__head">
                <h2 class="featured__head-h1">Fetured Items</h2>
                <h3 class="featured__head-h3">Shop for items based on what we featured in this week</h3>
            </div>

            <Catalog />

            <div class="featured__button">
                <a href="#" class="button">Browse All Product</a>
            </div>
        </section>

        <section class="offer center">
            <div class="offer__block">
                <h2 class="offer__block-h1">30% OFFER</h2>
                <h3 class="offer__block-h3">FOR WOMEN</h3>
            </div>
            <div class="offer__content">
                <div class="offer__content-flex">
                    <div class="offer__img">
                        <img src="../src/assets/img/offer_icon1.png" alt="" class="offer__icon">
                    </div>
                    <div class="offer__del-text offer__text-paddings">
                        <h3 class="offer__content-h3">Free Delivery</h3>
                        <p class="offer__content-p">Worldwide delivery on all. Authorit tively morph next-generation innov
                            tion with extensive models.</p>
                    </div>
                </div>
                <div class="offer__content-flex">
                    <div class="offer__img">
                        <img src="../src/assets/img/offer_icon2.png" alt="">
                    </div>
                    <div class="offer__sale-text offer__text-paddings">
                        <h3 class="offer__content-h3">Sales & discounts</h3>
                        <p class="offer__content-p">Worldwide delivery on all. Authorit tively morph next-generation innov
                            tion with extensive models.</p>
                    </div>
                </div>
                <div class="offer__content-flex">
                    <div class="offer__img">
                        <img src="../src/assets/img/offer_icon3.png" alt="">
                    </div>
                    <div class="offer__qual-text offer__text-paddings">
                        <h3 class="offer__content-h3">Quality assurance</h3>
                        <p class="offer__content-p">Worldwide delivery on all. Authorit tively morph next-generation innov
                            tion with extensive models.</p>
                    </div>
                </div>
            </div>
        </section>
        <div class="subscribe center">
            <div class="subscribe__human">
                <div class="subscribe__human-img"><img src="../src/assets/img/human.jpg" alt=""></div>
                <p class="subscribe__human-text">“Vestibulum quis porttitor dui! Quisque viverra nunc mi, a pulvinar purus
                    condimentum a. Aliquam condimentum mattis neque sed pretium”</p>
                <h3 class="subscribe__human-name">Bin Burhan</h3>
            </div>
            <div class="subscribe__form">
                <h1 class="subscribe__form-h1">Subscribe</h1>
                <h3 class="subscribe__form-h3">FOR OUR NEWLETTER AND PROMOTION</h3>
                <form action="#" class="subscribe__form-button">
                    <input id="email" placeholder="Enter Your Email" type="text" class="subscribe__email" required
                        pattern="\S+@[a-z]+.[a-z]+">
                    <input type="submit" class="subscribe__button" value="Subscribe">

                </form>
            </div>
        </div>
        <footer class="footer center">
            <div class="footer__left">
                <a class="logo" href="index.html">
                    <img class="logo__img" src="../src/assets/img/logo.png" alt="logo">BRAN<span class="accent">D</span>
                </a>
                <p class="footer__text">Objectively transition extensive data rather than cross functional solutions.
                    Monotonectally syndicate multidisciplinary materials before go forward benefits. Intrinsicly syndicate
                    an expanded array of processes and cross-unit partnerships. <br> <br> Efficiently plagiarize 24/365
                    action items
                    and focused infomediaries. Distinctively seize superior initiatives for wireless technologies.
                    Dynamically optimize. </p>
            </div>
            <div class="footer__right">
                <div class="footer__right-block">
                    <h1 class="footer__right-h1">COMPANY</h1>
                    <ul class="footer__list">
                        <li><a href="index.html" class="footer__link">Home</a></li>
                        <li><a href="#" class="footer__link">Shop </a></li>
                        <li><a href="#" class="footer__link">About </a></li>
                        <li><a href="#" class="footer__link">How It Works</a></li>
                        <li><a href="checkout.html" class="footer__link">Contact</a></li>
                    </ul>
                </div>
                <div class="footer__right-block">
                    <h1 class="footer__right-h1">INFORMATION</h1>
                    <ul class="footer__list">
                        <li><a href="#" class="footer__link">Tearms & Condition</a></li>
                        <li><a href="#" class="footer__link">Privacy Policy</a></li>
                        <li><a href="#" class="footer__link">How to Buy</a></li>
                        <li><a href="#" class="footer__link">How to Sell</a></li>
                        <li><a href="#" class="footer__link">Promotion</a></li>
                    </ul>
                </div>
                <div class="footer__right-block">
                    <h1 class="footer__right-h1">SHOP CATEGORY</h1>
                    <ul class="footer__list">
                        <li><a href="product.html" class="footer__link">Men</a></li>
                        <li><a href="single_page.html" class="footer__link">Women </a></li>
                        <li><a href="#" class="footer__link">Child</a></li>
                        <li><a href="#" class="footer__link">Apparel </a></li>
                        <li><a href="#" class="footer__link">Brows All</a></li>
                    </ul>
                </div>
            </div>
        </footer>
        <footer class="footer__line center">
            <div class="rights"> &copy;2017 Brand All Rights Reserved.</div>
            <div id="light" class="social">
                <ul class="social__list normal">
                    <li><a href="https://www.facebook.com/" class="btn-gradient facebook"><i
                                class="fa fa-facebook social__icon"></i></a></li>
                    <li><a href="https://twitter.com/explore" class="btn-gradient twitter"><i
                                class="fa fa-twitter social__icon"></i></a></li>
                    <li><a href="https://www.google.ru/" class="btn-gradient google-plus"><i
                                class="fa fa-google-plus social__icon"></i></a></li>
                    <li><a href="https://www.instagram.com" class="btn-gradient instagram"><i
                                class="fa fa-instagram social__icon"></i></a></li>
                    <li><a href="https://www.linkedin.com" class="btn-gradient linkedin"><i
                                class="fa fa-linkedin social__icon"></i></a></li>
                </ul>
            </div>
        </footer>
    </div>
</template>

<script>
import Catalog from './components/Catalog.vue';
import Basket from './components/Basket.vue';

export default {
    // components: { 'catalog-component': Catalog },
    components: { Catalog, Basket },
    data() {
        return {
            showBasket: false,
        }
    },
    methods: {
        _get(url) {
            return fetch(url).then(d => d.json())
        },  
    },
}
</script>

<style>

</style>