<template>
  <q-dialog
    v-model="isMenuOpen"
    transition-show="slide-left"
    transition-hide="slide-right"
    transition-duration="500"
    class="main-mob-dialog"
  >
    <q-card class="main-mob-dialog__block">
      <q-list class="main-mob-dialog__main-list">
        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
        <q-item
          clickable
          class="essential-link"
        >
          <q-item-section @click="router.push({name: 'registration'})">
            <q-item-label>Advertise with us</q-item-label>
          </q-item-section>
        </q-item>
        <q-item
          clickable
          class="essential-link"
        >
          <q-item-section @click="router.push({name: 'login'})">
            <q-item-label>Login</q-item-label>
          </q-item-section>
        </q-item>
      </q-list>
    </q-card>
  </q-dialog>
  <q-header class="main-header">
    <q-toolbar class="main-header__block container">
      <div class="main-header__logo">
        <router-link to="/">
          <img alt="logo" src="~assets/logo.svg" clickable/>
        </router-link>
      </div>
      <div class="main-header__nav">
        <q-list class="main-header__main-list">
          <EssentialLink
            v-for="link in essentialLinks"
            :key="link.title"
            v-bind="link"
          />
        </q-list>
        <q-list class="main-header__user-list">
          <q-btn class="main-btn main-btn--green main-btn--green--mini q-mr-sm" @click="router.push({name: 'registration'})">Advertise with us</q-btn>
          <q-btn class="main-btn main-btn--simple" @click="router.push({name: 'login'})">Login</q-btn>
        </q-list>
      </div>

      <q-btn
        flat
        dense
        round
        icon="menu"
        aria-label="Menu"
        color="black"
        class="main-header__menu-btn"
        @click="isMenuOpen=true"
      />
    </q-toolbar>
  </q-header>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import {useRouter} from 'vue-router';
import EssentialLink from 'components/EssentialLink.vue';

const router = useRouter();
const isMenuOpen = ref(false);

const essentialLinks = [
  {
    title: 'Advertisers and Agencies',
    link: '/'
  },
  {
    title: 'Publishers',
    link: '/pubs'
  },
  {
    title: 'Contacts',
    link: '/contacts'
  },
];

</script>
