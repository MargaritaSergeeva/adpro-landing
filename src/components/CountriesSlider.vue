<template>
  <div class="countries-slider">
    <swiper
      class="countries-slider__slider"
      :modules="[Navigation]"
      :speed="500"
      :navigation="{
        nextEl: '.countries-slider__next',
        prevEl: '.countries-slider__prev'
      }"
      :breakpoints="{
      '360': {
        slidesPerView: 3,
        spaceBetween: 15,
      },
      '768': {
        slidesPerView: 6,
        spaceBetween: 25,
      },
      '1300': {
        slidesPerView: 8,
        spaceBetween: 35,
      },
    }"
      loop
    >
      <swiper-slide v-for="country in countriesData" :key="country.id" class="countries-slider__slide">
        <q-card class="countries-slider__card">
          <img
            class="countries-slider__img"
            :src="'flags/' + country.img + '.svg'"
            :alt="country.img">
        </q-card>
      </swiper-slide>
    </swiper>
    <div class="countries-slider__prev"></div>
    <div class="countries-slider__next"></div>
  </div>


</template>

<script setup lang="ts">
import {Navigation} from 'swiper';
import {Swiper, SwiperSlide} from 'swiper/vue';
import AOS from 'aos';
import {onMounted} from 'vue';

onMounted(() => {
  AOS.init();
})

const countriesData = [
  {
    id: 1,
    img: 'id',
  },
  {
    id: 2,
    img: 'de',
  },
  {
    id: 3,
    img: 'my',
  },
  {
    id: 4,
    img: 'am',
  },
  {
    id: 5,
    img: 'th',
  },
  {
    id: 6,
    img: 'ua',
  },
  {
    id: 7,
    img: 'kaz',
  },
  {
    id: 8,
    img: 'lt',
  },
  {
    id: 9,
    img: 'ph',
  },
  {
    id: 10,
    img: 'cz',
  },
  {
    id: 11,
    img: 'it',
  }, {
    id: 12,
    img: 'ro',
  }, {
    id: 13,
    img: 'in',
  }, {
    id: 14,
    img: 'vn',
  },
  {
    id: 15,
    img: 'ee',
  },
  {
    id: 16,
    img: 'es',
  },
];
</script>
