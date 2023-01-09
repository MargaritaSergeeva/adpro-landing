<template>
  <q-page class="main-page">
    <section class="main-page__main-section main-section ">
      <div class="main-section__container container">
        <div class="main-section__text-block">
          <h1><span class="custom-font main-section__title main-title">AdProfex –</span> Native Advertising Platform</h1>
          <p class="main-section__text">More than <b>6 years</b> of experience <br>in the international advertising market</p>
          <q-btn class="main-btn main-btn--green main-btn--green--main main-btn--desktop" @click="router.push({name: 'contacts'})">Get presentation and cases</q-btn>
        </div>
        <div class="main-section__img-block">
          <div class="main-section__img-block-bg">
            <img class="main-section__img-block-figure1" src="~assets/main/main-rectangle-1.png" srcset="~assets/main/main-rectangle-1.png 1x, ~assets/main/main-rectangle-1-2x.png 2x" alt="rectangle-1">
            <img class="main-section__img-block-figure2" src="~assets/main/main-rectangle-2.svg" srcset="~assets/main/main-rectangle-2.png 1x, ~assets/main/main-rectangle-2-2x.png 2x" alt="rectangle-2">
            <img class="main-section__img-block-figure3" src="~assets/main/main-rectangle-3.svg" srcset="~assets/main/main-rectangle-3.png 1x, ~assets/main/main-rectangle-3-2x.png 2x" alt="rectangle-3">
            <img class="main-section__img-block-figure5" src="~assets/main/main-ellipse-1.svg" srcset="~assets/main/main-ellipse-1.png 1x, ~assets/main/main-ellipse-1-2x.png 2x" alt="ellipse-1">
            <img class="main-section__img-block-figure4" src="~assets/main/main-rectangle-4.svg" alt="rectangle-4">
            <img class="main-section__img-block-figure6" src="~assets/main/main-ellipse-2.svg" alt="ellipse-2">
            <img class="main-section__img-block-figure7" src="~assets/main/main-ellipse-3.svg" alt="ellipse-3">
            <img class="main-section__img-block-figure8" src="~assets/main/main-ellipse-4.svg" alt="ellipse-4">
          </div>
          <div class="main-section__img-block-content">
            <q-list class="main-section__img-block-list">
              <q-item class="main-section__img-block-item custom-font">
                <p>
                  <b class="main-section__img-block-text main-section__img-block-text--yellow">2&nbsp;million&nbsp;+</b>
                  <span>clicks daily</span>
                </p>
              </q-item>
              <q-item class="main-section__img-block-item custom-font">
                <p>
                  <b class="main-section__img-block-text">418 million</b>
                  <span>unique users</span>
                </p>
              </q-item>
              <q-item class="main-section__img-block-item custom-font">
                <p>
                  <b class="main-section__img-block-text">2760</b>
                  <span>own sites</span>
                </p>
                <p>
                  <b class="main-section__img-block-text custom-font">8050</b>
                  <span>partner sites</span>
                </p>
              </q-item>
              <q-item class="main-section__img-block-item custom-font">
                <p>
                  <b class="main-section__img-block-text">3 billion</b>
                  <span>ad block displays</span>
                </p>
              </q-item>
            </q-list>
          </div>
        </div>
        <q-btn class="main-btn main-btn--green main-btn--mob" @click="router.push({name: 'contacts'})">Get presentation and cases</q-btn>
      </div>
    </section>

    <section class="geo-section container">
      <h2 class="geo-section__title title custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Broad GEO coverage</h2>
      <p class="geo-section__intro intro" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">We offer advertisers quality native traffic from more than 22 countries</p>
      <div class="geo-section__slider-block" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
        <GeoSlider/>
      </div>
    </section>

    <section class="targeting-section">
      <div class="targeting-section__container container">
        <h2 class="targeting-section__title title title--white custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Configuration and targeting</h2>
        <p class="targeting-section__intro intro intro--white" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">TGB • TGB In-Read • Banner</p>
        <div class="targeting-section__desktop" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            <TargetingSlider/>
        </div>
        <div class="targeting-section__mob" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
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
        <p class="targeting-section__intro intro intro--white intro--bold" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Available Target Settings</p>
        <q-list class="targeting-section__target-list" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <q-item class="targeting-section__target-item"><p>Geography</p></q-item>
          <q-item class="targeting-section__target-item"><p>Devices <br>(PC/Mob)</p></q-item>
          <q-item class="targeting-section__target-item"><p>Operating systems</p></q-item>
          <q-item class="targeting-section__target-item"><p>Telecom operators</p></q-item>
          <q-item class="targeting-section__target-item"><p>Browsers</p></q-item>
        </q-list>
        <q-list class="targeting-section__target-list-big" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <q-item class="targeting-section__target-item-big">
            <p>Integration with DMP platforms</p>
            <ul>
              <li>AmberData</li>
              <li>Weborama and others</li>
            </ul>
          </q-item>
          <q-item class="targeting-section__target-item-big targeting-section__target-item-big--wide">
            <p>Audience data</p>
            <ul>
              <li>Society/Demography (gender/age)</li>
              <li>Interests/hobby</li>
              <li>Retargeting, LAL</li>
            </ul>
          </q-item>
          <q-item class="targeting-section__target-item-big targeting-section__target-item-big--extra">
            <p>Keywords</p>
            <span>
              Articles with necessary key words
            </span>
          </q-item>
          <q-item class="targeting-section__target-item-big targeting-section__target-item-big--extra">
            <p>Sites/Platforms list</p>
            <span>
              Thematic sites/platforms selection
            </span>
          </q-item>
        </q-list>
        <q-btn
          class="targeting-section__main-btn main-btn main-btn--green main-btn--wide"
          data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true"
          @click="router.push({name: 'registration'})"
        >
          Advertise with us
        </q-btn>
      </div>
    </section>

    <section class="advantages-section container">
      <h2 class="advantages-section__title title custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Advantages of working with AdProfex for advertisers and agencies</h2>
      <q-list class="advantages-section__list">
        <q-item class="advantages-section__item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <p>The <b>cost</b> of advertising is lower than that of competitors</p>
        </q-item>
        <q-item class="advantages-section__item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <p>Profitable purchase using <b>Cross-device targeting</b> technology, which allows you to catch one user on different devices</p>
        </q-item>
        <q-item class="advantages-section__item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <p><b>Targeting 200 +:</b> socio-demographic; contextual; interests of users; in keywords</p>
        </q-item>
        <q-item class="advantages-section__item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <p>Over <b>2760</b> own sites <br><b>+ 8050</b> partner sites</p>
        </q-item>
        <q-item class="advantages-section__item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <p><b>Quality</b>  control and of advertising viewability</p>
        </q-item>
        <q-item class="advantages-section__item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <p>Accept <b>any</b> verifiers and trackers</p>
        </q-item>
        <q-item class="advantages-section__item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <p>Complete work <b>transparency</b></p>
        </q-item>
        <q-item class="advantages-section__item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <p>Creatives as a <b>bonus</b>, adaptive configurations</p>
        </q-item>
        <q-item class="advantages-section__item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <p><b>Purchasing</b> forms срс, срм, vcpm</p>
        </q-item>
      </q-list>
    </section>

    <section class="faq-section">
      <div class="faq-section__container container">
        <h2 class="faq-section__title title custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">FAQ</h2>
        <q-list class="faq-section__list" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <q-expansion-item
            expand-separator
            label="What formats/configurations do you provide with?"
            class="faq-section__accordion"
            expand-icon="add"
            expanded-icon="remove"

          >
            <q-card>
              <q-card-section>
                At the moment, we have three formats: TGB, TGB In-Read, banner.
              </q-card-section>
            </q-card>
          </q-expansion-item>
          <q-expansion-item
            expand-separator
            label="What are the technical requirements?"
            class="faq-section__accordion"
            expand-icon="add"
            expanded-icon="remove"

          >
            <q-card>
              <q-card-section>
                <p><b>To TGB</b></p>
                <p>The advertising format is located under the article or on the side</p>
                <p>100 character header</p>
                <p>Files in JPG and PNG are supported for images</p>
                <p>You can crop an image when you create a creative</p>
                <p>The maximum size of a square image is 367x367px</p>
                <p>Maximum rectangular image size - 539x359px</p>
                <p><b>To TGB In-Read</b></p>
                <p>The advertising format is located inside the text, it is automatically scaled for the mobile version. It can combine the following elements: image, title, description and button.</p>
                <p>Valid image sizes:</p>
                <p>300*300, 400*400, 305*240, 300*250, 300*409, 250*200, 320*270</p>
                <p>345*345, 345*200, 400*400, 400*350, 335*224, 250*300, 250*400, 240*250, 240*300, 500*455, 500*310, 500*240, 345*230, 600*336, 790*520, 376*376</p>
                <p>Text ads do not allow abuse of Caps-Lock and exclamation/question marks. Each sentence must end with a punctuation mark: full stop, exclamation mark or question mark.</p>
                <p>A text declaration can consist of the following elements:</p>
                <p>Title - no more than 65 characters, recommended 25.</p>
                <p>Description - no more than 90 characters, recommended 75.</p>
                <p>The main image is the dimensions cm above, preferably 3-4 sizes</p>
                <p>Call to Action: text on the button, for example: More details, Install, Download, etc. No more than 15 characters, recommended 10.</p>
                <p><b>To banners</b></p>
                <p>Image formats: PNG (.png), GIF (.gif), JPEG (.jpeg).</p>
                <p><b>The main allowable dimensions are:</b></p>
                <p>For phones: 320x50, 320x100, 300x250, 300х300, 300x600, 240x400, 320x480, 480x320, 970x90, 970x250, 336x280, 728x90, 468x60, 160х600</p>
                <p>For PC: 728x90, 240x400, 300x250, 468x60, 160x600, 336x280, 300x600, 300х300, 970x250, 1000x120, 970х90</p>
                <p>For tablets: 320x50, 320x100, 300x250, 300х300, 300x600, 240x400, 320x480, 480x320, 970x90, 970x250, 336x280, 728x90, 468x60, 160х600</p>
                <p><b>Additional dimensions:</b></p>
                <p>For phones: 300x500, 240x600, 300x50, 300x100, 375x50, 200x200, 250x250</p>
                <p>For PC: 320x100, 300x500, 120x600, 200х300, 980x120, 980x90</p>
                <p>For tablets: 768x1024, 1024x768, 640x360, 360x640</p>
                <p>Recommended rules for creating HTML banners:</p>
                <ul>
                  <li>The banner must be an archive of many files: index.html and sprite.png (two and no more than 100 are recommended). Only relative references to resource files are allowed in the index.html file.</li>
                  <li>Be sure to reduce the size of sprite.png files through the service https://tinypng.com/</li>
                  <li>In an index.html file, base64 views for images are not allowed.</li>
                </ul>
                <p>All clicks of events that cause a switch to an advertiser's site must be handled strictly through the &lt;a href=””&gt;</p>
              </q-card-section>
            </q-card>
          </q-expansion-item>
          <q-expansion-item
            expand-separator
            label="What targets are available?"
            class="faq-section__accordion"
            expand-icon="add"
            expanded-icon="remove"

          >
            <q-card>
              <q-card-section>
                <p>At the moment, it is possible to target:</p>
                <ul>
                  <li>GEO</li>
                  <li>Devices (PC/mobile)</li>
                  <li>Browsers</li>
                  <li>Operating systems</li>
                  <li>Telecom operators</li>
                  <li>Audience data</li>
                  <li>Social demography (gender/age)</li>
                  <li>AdProfex Interests - Native data based on content consumption</li>
                  <li>Third-party data: AmberData, Weborama</li>
                  <li>Retargeting, Look-alike</li>
                </ul>
              </q-card-section>
            </q-card>
          </q-expansion-item>
          <q-expansion-item
            expand-separator
            label="Which counters does the platform support?"
            class="faq-section__accordion"
            expand-icon="add"
            expanded-icon="remove"

          >
            <q-card>
              <q-card-section>
                We accept any counters of different systems.
              </q-card-section>
            </q-card>
          </q-expansion-item>
        </q-list>
        <q-btn
          class="faq-section__main-btn main-btn main-btn--green main-btn--wide"
          data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true"
          @click="router.push({name: 'registration'})">
          Advertise with us
        </q-btn>
      </div>
    </section>

    <section class="features-section">
      <div class="features-section__container container">
        <h2 class="features-section__title title custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Unique proprietary RTB engine and technologies</h2>
        <q-list class="features-section__list" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
          <q-item class="features-section__item">
            <p>
              more than <b>15,000</b> own sites, which allows you to purchase inventory without surcharges
            </p>
          </q-item>
          <q-item class="features-section__item">
            <p>
              <b>integration</b> with international trackers and verifiers
            </p>
          </q-item>
          <q-item class="features-section__item">
            <p>
              possibility of <b>purchasing model</b> selection (SRS, SRM, vCPM)
            </p>
          </q-item>
          <q-item class="features-section__item">
            <p>
              automatic <b>optimization of creatives</b> (adjustment for content)
            </p>
          </q-item>
          <q-item class="features-section__item">
            <p>
              <b>real-time</b> statistics
            </p>
          </q-item>
          <q-item class="features-section__item features-section__item--big">
            <p>
              <b>all formats</b> are available - native, banners, video
            </p>
          </q-item>
        </q-list>
      </div>
    </section>

    <section class="control-section">
      <div class="control-section__container container">
        <h2 class="control-section__title title title--white custom-font" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Advertising placement control</h2>
        <p class="control-section__intro intro intro--bold intro--white" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">Brand safety</p>
        <div class="control-section__block">
          <div class="control-section__block-item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            <h3 >Fraud and unnecessary content brands’ protection</h3>
            <q-list class="control-section__block-list">
              <q-item class="control-section__block-list-item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
                <p>Brand protection from fraud and unnecessary content</p>
              </q-item>
              <q-item class="control-section__block-list-item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
                <p>Context filters</p>
              </q-item>
              <q-item class="control-section__block-list-item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
                <p>Black lists</p>
              </q-item>
              <q-item class="control-section__block-list-item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
                <p>Manual optimization of each advertising campaign</p>
              </q-item>
              <q-item class="control-section__block-list-item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
                <p>Filtering by keywords, page content</p>
              </q-item>
            </q-list>
          </div>
          <div class="control-section__block-item" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
            <h3 >High quality of our traffic confirmed</h3>
            <div class="control-section__block-sign" >
              <p>Antifrod A</p>
            </div>
            <p>Proprietary Fraud Protection System - Antifrod A</p>
            <div class="control-section__block-imgs" data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true">
              <img class="control-section__block-img" src="~assets/main/weborama.jpg" srcset="~assets/main/weborama.jpg 1x, ~assets/main/weborama-2x.jpg 2x" alt="weborama">
              <img class="control-section__block-img" src="~assets/main/adriver.jpg" srcset="~assets/main/adriver.jpg 1x, ~assets/main/adriver-2x.jpg 2x" alt="adriver">
              <img class="control-section__block-img" src="~assets/main/sizmek.jpg" srcset="~assets/main/sizmek.jpg 1x, ~assets/main/sizmek-2x.jpg 2x" alt="sizmek">
            </div>
            <p>Application of third party verifiers: Weborama, AdRiver, Sizmek and others</p>
          </div>
        </div>
        <q-btn
          class="control-section__main-btn main-btn main-btn--green main-btn--wide"
          data-aos="fade-up" data-aos-anchor-placement="top-center" data-aos-duration="1000" data-aos-once="true"
          @click="router.push({name: 'registration'})"
        >
          Advertise with us
        </q-btn>
      </div>
    </section>
  </q-page>
</template>

<script setup lang="ts">
import { onMounted } from 'vue';
import GeoSlider from 'components/GeoSlider.vue';
import TargetingSlider from 'components/TargetingSlider.vue';
const AOS = require('aos');
import {useRouter} from 'vue-router';

const router = useRouter();

onMounted(() => {
  AOS.init();
})
</script>
