<template>
  <q-page class="pubs-page">
    <section class="pubs-page__main-section pubs-main-section ">
      <div class="pubs-main-section__container container">
        <div class="pubs-main-section__wrapper">
          <div class="pubs-main-section__text-block">
            <h1 class="custom-font pubs-main-section__title page-title">Earn more with AdProfex ad network</h1>
            <p class="pubs-main-section__text">We provide opportunities for simple and profitable monetization of a site of any size.</p>
            <p class="pubs-main-section__text">We are pleased to collaborate with both large publishers and owners of small sites.</p>
          </div>
          <div class="pubs-main-section__img-block">
            <div class="pubs-main-section__img-block-bg">
              <img class="pubs-main-section__img-block-figure1" src="~assets/pubs/pubs-ellipse1.png" srcset="~assets/pubs/pubs-ellipse1.png 1x, ~assets/pubs/pubs-ellipse1-2x.png 2x" alt="ellipse1">
              <img class="pubs-main-section__img-block-figure2" src="~assets/pubs/pubs-ellipse2.png" srcset="~assets/pubs/pubs-ellipse2.png 1x, ~assets/pubs/pubs-ellipse2-2x.png 2x" alt="ellipse2">
              <img class="pubs-main-section__img-block-figure3" src="~assets/pubs/pubs-rectangle1.png" srcset="~assets/pubs/pubs-rectangle1.png 1x, ~assets/pubs/pubs-rectangle1-2x.png 2x" alt="rectangle-3">
              <img class="pubs-main-section__img-block-figure4" src="~assets/pubs/pubs-rectangle2.svg" alt="rectangle2">
              <img class="pubs-main-section__img-block-figure5" src="~assets/pubs/pubs-rectangle1.svg" alt="rectangle1">
              <img class="pubs-main-section__img-block-figure6" src="~assets/pubs/pubs-ellipse.svg" alt="ellipse1">
              <img class="pubs-main-section__img-block-figure7" src="~assets/pubs/tisers.png" srcset="~assets/pubs/tisers.png 1x, ~assets/pubs/tisers-2x.png 2x" alt="rectangle3">
            </div>
          </div>
        </div>
        <q-btn class="pubs-main-section__main-btn main-btn main-btn--green" @click="router.push({name: 'registration'})">Start earning with us</q-btn>
      </div>
    </section>
    <section class="countries-section container">
      <h2 class="countries-section__title title custom-font">Countries we cooperate with</h2>
      <div>
        <CountriesSlider/>
      </div>
    </section>

    <section class="targeting-section targeting-section--pubs">
      <div class="targeting-section__container container">
        <h2 class="targeting-section__title title title--white custom-font">Configuration</h2>
        <p class="targeting-section__intro intro intro--white">TGB • TGB In-Read</p>
        <div class="targeting-section__desktop">
          <TargetingSlider/>
        </div>
        <div class="targeting-section__mob">
          <q-list class="targeting-section__mob-list">
            <q-item class="targeting-section__mob-item">
              <picture>
                <img class="targeting-section__mob-img" src="~assets/main/begining-article.png" srcset="~assets/main/begining-article.png 1x, ~assets/main/begining-article-2x.png 2x" alt="begining article">
              </picture>
              <p class="targeting-section__mob-text">At the beginning of the article</p>
            </q-item>
            <q-item class="targeting-section__mob-item">
              <picture>
                <img class="targeting-section__mob-img" src="~assets/main/ending-article.png" srcset="~assets/main/ending-article.png 1x, ~assets/main/ending-article-2x.png 2x" alt="ending article">
              </picture>
              <p class="targeting-section__mob-text">At the end of the article</p>
            </q-item>
            <q-item class="targeting-section__mob-item">
              <picture>
                <img class="targeting-section__mob-img" src="~assets/main/middle-article.png" srcset="~assets/main/middle-article.png 1x, ~assets/main/middle-article-2x.png 2x" alt="middle article">
              </picture>
              <p class="targeting-section__mob-text">In the middle of the article</p>
            </q-item>
            <q-item class="targeting-section__mob-item">
              <picture>
                <img class="targeting-section__mob-img" src="~assets/main/side-article.png" srcset="~assets/main/side-article.png 1x, ~assets/main/side-article-2x.png 2x" alt="side article">
              </picture>
              <p class="targeting-section__mob-text">On the right sidebar</p>
            </q-item>
          </q-list>
        </div>
      </div>
    </section>
  </q-page>
</template>

<script setup lang="ts">
import CountriesSlider from 'src/components/CountriesSlider.vue';
import TargetingSlider from 'components/TargetingSlider.vue';

</script>
