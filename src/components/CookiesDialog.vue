<template>
  <q-dialog
    v-model="isCookiesDialogOpen"
    class="cookies-dialog"
    seamless
    transition-show="slide-up"
    transition-hide="slide-down"
    transition-duration="800"
  >
    <q-tab-panels
      v-model="tab"
      animated
      swipeable
      vertical
      transition-prev="jump-up"
      transition-next="jump-up"
    >
      <q-tab-panel name="firstTab">
        <div class="cookies-dialog__first-tab">
          <div class="cookies-dialog__first-tab-text">
            <h3 class="custom-font">We use cookies</h3>
            <p>to improve your experience</p>
            <a href="#">Show cookie policy</a>
          </div>
          <div class="cookies-dialog__first-tab-btns">
            <q-btn
              class="main-btn main-btn--green main-btn--transparent main-btn--wide"
              @click="tab='secondTab'"
            >
              Manage preferences
            </q-btn>
            <q-btn
              class="main-btn main-btn--green main-btn--wide"
              @click="isCookiesDialogOpen=false"
            >
              Accept all
            </q-btn>
          </div>
        </div>
      </q-tab-panel>

      <q-tab-panel name="secondTab">
        <div class="cookies-dialog__second-tab">
          <q-btn class="cookies-dialog__close-btn" flat round color="grey" icon="close" @click="tab='firstTab'"/>
          <h3 class="custom-font">Your cookie preferences</h3>
          <p class="cookies-dialog__second-tab-text">We use cookies to ensure basic functionality of the website and to
            enhance your online experience. For each category, you may choose to opt-in/out whenever you want.</p>
          <a href="#">Cookie policy</a>
          <div class="cookies-dialog__expansion-item-block">
            <q-expansion-item
              switch-toggle-side
              label="Strictly necessary cookies"
            >
              <q-card>
                <q-card-section>
                  These cookies are essential for the proper functioning of this website. They do not contain personal
                  data and are not used to track you.
                </q-card-section>
              </q-card>
            </q-expansion-item>
            <q-expansion-item
              switch-toggle-side
            >
              <template v-slot:header>
                <q-item-section>
                  Google Services
                </q-item-section>
                <q-item-section side>
                  <q-toggle
                    v-model="googleServicesCookies"
                  />
                </q-item-section>
              </template>
              <q-card>
                <q-card-section>
                  <p>Allows the integration and usage of Google services.</p>
                  <p><b>Used services</b></p>
                  <div class="cookies-dialog__expansion-item-side">
                    <p>Google Analytics</p>
                    <a href="#">Display policies</a>
                  </div>
                </q-card-section>
              </q-card>
            </q-expansion-item>
          </div>

          <div class="cookies-dialog__second-tab-btns">
            <q-btn
              class="main-btn main-btn--green main-btn--transparent main-btn--wide"
              @click="isCookiesDialogOpen=false"
            >
              Save preferences
            </q-btn>
            <q-btn
              class="main-btn main-btn--green main-btn--wide"
              @click="isCookiesDialogOpen=false"
            >
              Accept all
            </q-btn>
          </div>
        </div>
      </q-tab-panel>
    </q-tab-panels>
  </q-dialog>
</template>

<script setup lang="ts">
import {ref} from 'vue';

const isCookiesDialogOpen = ref(true);
const tab = ref('firstTab');
const googleServicesCookies = ref(true);
</script>
