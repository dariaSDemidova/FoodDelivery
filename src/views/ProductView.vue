<template>
    <section class="products">
        <div class="container">
            <div class="products-header">
                <h2 class="products-header--title">
                    Тануки
                </h2>
            </div>
            <div class="products-wrapper" id="products-container">
                <div class="products-card" v-for="product in productsArray" :key="product.id">
                            <div class="products-card__image">
                                <img :src="getUrl(product.image)" alt="product">
                            </div>
                            <div class="products-card__description">
                                <div class="products-card__description-row">
                                    <h3 class="products-card__description--name">{{product.name}}</h3>
                                </div>
                                <div class="products-card__description-row">
                                    <p class="products-card__description--text">{{product.text}}</p>
                                </div>
                                <div class="products-card__description-row">
                                    <div class="products-card__description-controls">
                                        <button class="btn btn-primary">
                                            В корзину
                                            <img src="../assets/images/icons/shopping-cart-white.svg" alt="shopping-cart">
                                        </button>
                                <span class="products-card__description-controls--price">{{product.price}} ₽</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import {productsArray} from '../constants/products'

const getUrl = (name) => {
    return new URL(`../assets/images/goods/${name}`, import.meta.url)
}

</script>
