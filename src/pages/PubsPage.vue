<template>
  <q-page class="pubs-page">
    <section class="pubs-page__main-section pubs-main-section ">
      <div class="pubs-main-section__container container">
        <div class="pubs-main-section__wrapper">
          <div class="pubs-main-section__text-block">
            <h1 class="custom-font pubs-main-section__title page-title">Earn more with AdProfex ad network</h1>
            <p class="pubs-main-section__text">We provide opportunities for simple and profitable monetization of a site
              of any size.</p>
            <p class="pubs-main-section__text">We are pleased to collaborate with both large publishers and owners of
              small sites.</p>
          </div>
          <div class="pubs-main-section__img-block">
            <div class="pubs-main-section__img-block-bg">
              <img class="pubs-main-section__img-block-figure1" src="~assets/pubs/pubs-ellipse1.png"
                   srcset="~assets/pubs/pubs-ellipse1.png 1x, ~assets/pubs/pubs-ellipse1-2x.png 2x" alt="ellipse1">
              <img class="pubs-main-section__img-block-figure2" src="~assets/pubs/pubs-ellipse2.png"
                   srcset="~assets/pubs/pubs-ellipse2.png 1x, ~assets/pubs/pubs-ellipse2-2x.png 2x" alt="ellipse2">
              <img class="pubs-main-section__img-block-figure3" src="~assets/pubs/pubs-rectangle1.png"
                   srcset="~assets/pubs/pubs-rectangle1.png 1x, ~assets/pubs/pubs-rectangle1-2x.png 2x"
                   alt="rectangle-3">
              <img class="pubs-main-section__img-block-figure4" src="~assets/pubs/pubs-rectangle2.svg" alt="rectangle2">
              <img class="pubs-main-section__img-block-figure5" src="~assets/pubs/pubs-rectangle1.svg" alt="rectangle1">
              <img class="pubs-main-section__img-block-figure6" src="~assets/pubs/pubs-ellipse.svg" alt="ellipse1">
              <img class="pubs-main-section__img-block-figure7" src="~assets/pubs/tisers.png"
                   srcset="~assets/pubs/tisers.png 1x, ~assets/pubs/tisers-2x.png 2x" alt="rectangle3">
            </div>
          </div>
        </div>
        <q-btn class="pubs-main-section__main-btn main-btn main-btn--green"
               @click="router.push({name: 'registration'})">Start earning with us
        </q-btn>
      </div>
    </section>
    <section class="countries-section container">
      <h2 class="countries-section__title title custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Countries we cooperate with</h2>
      <div data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
        <CountriesSlider/>
      </div>
    </section>

    <section class="targeting-section targeting-section--pubs">
      <div class="targeting-section__container container">
        <h2 class="targeting-section__title title title--white custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Configuration</h2>
        <p class="targeting-section__intro intro intro--white" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">TGB • TGB In-Read</p>
        <div class="targeting-section__desktop" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <TargetingSlider/>
        </div>
        <div class="targeting-section__mob" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <q-list class="targeting-section__mob-list">
            <q-item class="targeting-section__mob-item">
              <picture>
                <img class="targeting-section__mob-img" src="~assets/main/begining-article.png"
                     srcset="~assets/main/begining-article.png 1x, ~assets/main/begining-article-2x.png 2x"
                     alt="begining article">
              </picture>
              <p class="targeting-section__mob-text">At the beginning of the article</p>
            </q-item>
            <q-item class="targeting-section__mob-item">
              <picture>
                <img class="targeting-section__mob-img" src="~assets/main/ending-article.png"
                     srcset="~assets/main/ending-article.png 1x, ~assets/main/ending-article-2x.png 2x"
                     alt="ending article">
              </picture>
              <p class="targeting-section__mob-text">At the end of the article</p>
            </q-item>
            <q-item class="targeting-section__mob-item">
              <picture>
                <img class="targeting-section__mob-img" src="~assets/main/middle-article.png"
                     srcset="~assets/main/middle-article.png 1x, ~assets/main/middle-article-2x.png 2x"
                     alt="middle article">
              </picture>
              <p class="targeting-section__mob-text">In the middle of the article</p>
            </q-item>
            <q-item class="targeting-section__mob-item">
              <picture>
                <img class="targeting-section__mob-img" src="~assets/main/side-article.png"
                     srcset="~assets/main/side-article.png 1x, ~assets/main/side-article-2x.png 2x" alt="side article">
              </picture>
              <p class="targeting-section__mob-text">On the right sidebar</p>
            </q-item>
          </q-list>
        </div>
      </div>
    </section>

    <section class="ad-efficiency">
      <h2 class="ad-efficiency__title title custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">New Ad efficiency</h2>
      <div class="ad-efficiency__container container">
        <div class="ad-efficiency__block">
          <div class="ad-efficiency__inner">
            <img class="ad-efficiency__img" src="~assets/pubs/content-blackout.svg" alt="Content blackout" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            <h3 class="ad-efficiency__inner-title" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Content blackout</h3>
          </div>
          <p class="ad-efficiency__inner-text" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            This block could raise yields by 25%. When a block appears on the user's screen, all content around is
            darkened and attention is focused on advertising, thereby causing a desire to click on this block. Due to
            this, CTR and your income are growing.
          </p>
        </div>
        <div class="ad-efficiency__block">
          <div class="ad-efficiency__inner">
            <img class="ad-efficiency__img" src="~assets/pubs/autoload.svg" alt="Auto load" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            <h3 class="ad-efficiency__inner-title" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Auto-load of teasers</h3>
          </div>
          <p class="ad-efficiency__inner-text" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            Put the block at the end of the article and as soon as the user gets to it - he will load new blocks with
            ads, thereby allowing the user to see more ads, increasing the likelihood of a click.
          </p>
        </div>
      </div>
    </section>
    <section class="personal-acc">
      <h2 class="personal-acc__title title custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Convenient personal account</h2>
      <div class="personal-acc__container container">
        <div class="personal-acc__block">
          <h3 class="personal-acc__inner-title" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Block constructor</h3>
          <q-list class="personal-acc__list" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            <q-item class="personal-acc__item">Perform automatic A/B tests in a few clicks;</q-item>
            <q-item class="personal-acc__item">More than 20 ready-made adaptive templates.</q-item>
          </q-list>
        </div>
        <div class="personal-acc__block">
          <h3 class="personal-acc__inner-title" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Detailed analytics</h3>
          <p class="personal-acc__inner-text" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Analyze income by a variety of parameters:</p>
          <q-list class="personal-acc__inner-list" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            <q-item class="personal-acc__inner-item">Websites</q-item>
            <q-item class="personal-acc__inner-item">Blocks</q-item>
            <q-item class="personal-acc__inner-item">Devices</q-item>
            <q-item class="personal-acc__inner-item">Countries</q-item>
          </q-list>
        </div>
        <div class="personal-acc__block">
          <h3 class="personal-acc__inner-title" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Finance</h3>
          <q-list class="personal-acc__list" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            <q-item class="personal-acc__item">Compliance with the EDR</q-item>
            <q-item class="personal-acc__item">Convenient payments including to the current account</q-item>
            <q-item class="personal-acc__item">Compliance with tax legislation</q-item>
          </q-list>
        </div>
      </div>
      <q-btn class="personal-acc__main-btn main-btn main-btn--green"
             data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true"
             @click="router.push({name: 'registration'})">Try our service
      </q-btn>
    </section>
    <section class="offer">
      <h2 class="offer__title title title--white custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">We offer</h2>
      <div class="offer__container container">
        <q-list class="offer__list" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <q-item class="offer__item">High quality advertising</q-item>
          <q-item class="offer__item">Convenient ways of outputting income</q-item>
          <q-item class="offer__item">A wide selection of high-yield templates</q-item>
          <q-item class="offer__item">Bypassing automatic ad blocking systems</q-item>
          <q-item class="offer__item">Technical support 24/7</q-item>
        </q-list>
        <q-btn class="offer__main-btn main-btn main-btn--green"
               data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true"
               @click="router.push({name: 'registration'})">Register
        </q-btn>
      </div>
    </section>
  </q-page>
</template>

<script setup lang="ts">
import {useRouter} from 'vue-router';
import CountriesSlider from 'src/components/CountriesSlider.vue';
import TargetingSlider from 'components/TargetingSlider.vue';

const router = useRouter();
</script>
