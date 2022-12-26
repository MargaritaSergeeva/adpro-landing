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
      <h2 class="geo-section__title title custom-font">Broad GEO coverage</h2>
      <p class="geo-section__intro intro">We offer advertisers quality native traffic from more than 22 countries</p>
      <div class="geo-section__slider-block">
        <GeoSlider/>
      </div>
    </section>

    <section class="targeting-section">
      <div class="targeting-section__container container">
        <h2 class="targeting-section__title title title--white custom-font" >Configuration and targeting</h2>
        <p class="targeting-section__intro intro intro--white" >TGB • TGB In-Read • Banner</p>
        <div class="targeting-section__desktop" >
            <TargetingSlider/>
        </div>
        <div class="targeting-section__mob" >
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
        <p class="targeting-section__intro intro intro--white intro--bold" >Available Target Settings</p>
        <q-list class="targeting-section__target-list" >
          <q-item class="targeting-section__target-item"><p>Geography</p></q-item>
          <q-item class="targeting-section__target-item"><p>Devices <br>(PC/Mob)</p></q-item>
          <q-item class="targeting-section__target-item"><p>Operating systems</p></q-item>
          <q-item class="targeting-section__target-item"><p>Telecom operators</p></q-item>
          <q-item class="targeting-section__target-item"><p>Browsers</p></q-item>
        </q-list>
        <q-list class="targeting-section__target-list-big" >
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
        >
          Advertise with us
        </q-btn>
      </div>
    </section>

    <section class="advantages-section container">
      <h2 class="advantages-section__title title custom-font" >Advantages of working with AdProfex for advertisers and agencies</h2>
      <q-list class="advantages-section__list">
        <q-item class="advantages-section__item" >
          <p>The <b>cost</b> of advertising is lower than that of competitors</p>
        </q-item>
        <q-item class="advantages-section__item" >
          <p>Profitable purchase using <b>Cross-device targeting</b> technology, which allows you to catch one user on different devices</p>
        </q-item>
        <q-item class="advantages-section__item" >
          <p><b>Targeting 200 +:</b> socio-demographic; contextual; interests of users; in keywords</p>
        </q-item>
        <q-item class="advantages-section__item" >
          <p>Over <b>2760</b> own sites <br><b>+ 8050</b> partner sites</p>
        </q-item>
        <q-item class="advantages-section__item" >
          <p><b>Quality</b>  control and of advertising viewability</p>
        </q-item>
        <q-item class="advantages-section__item" >
          <p>Accept <b>any</b> verifiers and trackers</p>
        </q-item>
        <q-item class="advantages-section__item" >
          <p>Complete work <b>transparency</b></p>
        </q-item>
        <q-item class="advantages-section__item" >
          <p>Creatives as a <b>bonus</b>, adaptive configurations</p>
        </q-item>
        <q-item class="advantages-section__item" >
          <p><b>Purchasing</b> forms срс, срм, vcpm</p>
        </q-item>
      </q-list>
    </section>

  </q-page>
<!--    <section class="faq-section container">-->
<!--      <h2 class="faq-section__title title custom-font" >FAQ</h2>-->
<!--      <q-list class="faq-section__list">-->
<!--        <q-expansion-item-->
<!--          expand-separator-->
<!--          label="Какие форматы есть?"-->
<!--          class="faq-section__accordion"-->
<!--          expand-icon="add"-->
<!--          expanded-icon="remove"-->
<!--          -->
<!--        >-->
<!--          <q-card>-->
<!--            <q-card-section>-->
<!--              На данный момент у нас присутствуют три формата: <b>TGB, TGB In-Read, баннер.</b>-->
<!--            </q-card-section>-->
<!--          </q-card>-->
<!--        </q-expansion-item>-->
<!--        <q-expansion-item-->
<!--          expand-separator-->
<!--          label="Какие технические требования?"-->
<!--          class="faq-section__accordion"-->
<!--          expand-icon="add"-->
<!--          expanded-icon="remove"-->
<!--          -->
<!--        >-->
<!--          <q-card>-->
<!--            <q-card-section>-->
<!--              <p><b>К TGB</b></p>-->
<!--              <p>Рекламный формат располагается под статьей или сбоку.</p>-->
<!--              <p>Заголовок 100 символов.</p>-->
<!--              <p>Для изображений поддерживаются файлы в JPG и PNG.</p>-->
<!--              <p>Изображение можно обрезать при создании креатива.</p>-->
<!--              <p>Максимальный размер квадратного изображения – 367х367px</p>-->
<!--              <p>Максимальный размер прямоугольного изображения – 539х359px</p>-->
<!--              <p><b>К TGB In-Read</b></p>-->
<!--              <p>Рекламный формат располагается внутри текста, автоматически масштабируется под мобильную версию. Может комбинировать в себе следующие элементы: изображение, заголовок, описание и кнопка.</p>-->
<!--              <p>Допустимые размеры изображений :</p>-->
<!--              <p>300*300, 400*400, 305*240, 300*250, 300*409, 250*200, 320*270</p>-->
<!--              <p>345*345, 345*200, 400*400, 400*350, 335*224, 250*300, 250*400, 240*250, 240*300, 500*455, 500*310, 500*240, 345*230, 600*336, 790*520, 376*376</p>-->
<!--              <p>В текстовых объявлениях не разрешаются злоупотребления Caps-Lock и восклицательными/вопросительными знаками. Каждое предложение должно заканчиваться знаком препинания: точка, восклицательный или вопросительный знаки.</p>-->
<!--              <p>Текстовое объявление может состоять из следующих элементов:</p>-->
<!--              <p>Заголовок - Не более 65 символов, рекомендовано 25.</p>-->
<!--              <p>Описание - Не более 90 символов, рекомендовано 75.</p>-->
<!--              <p>Главное изображение - размеры см выше, желательно 3-4 размера.</p>-->
<!--              <p>Call to Action: текст на кнопке, например: Подробнее, Установить, Скачать и др. Не более 15 символов, рекомендовано 10.</p>-->
<!--              <p><b>К баннерам</b></p>-->
<!--              <p>Форматы изображений: PNG (.png), GIF (.gif), JPEG (.jpeg).</p>-->
<!--              <p><b>Основные допустимые размеры:</b></p>-->
<!--              <p>Для телефонов: 320x50, 320x100, 300x250, 300х300, 300x600, 240x400, 320x480, 480x320, 970x90, 970x250, 336x280, 728x90, 468x60, 160х600</p>-->
<!--              <p>Для ПК: 728x90, 240x400, 300x250, 468x60, 160x600, 336x280, 300x600, 300х300, 970x250, 1000x120, 970х90</p>-->
<!--              <p>Для планшетов: 320x50, 320x100, 300x250, 300х300, 300x600, 240x400, 320x480, 480x320, 970x90, 970x250, 336x280, 728x90, 468x60, 160х600</p>-->
<!--              <p><b>Дополнительные размеры:</b></p>-->
<!--              <p>Для телефонов: 300x500, 240x600, 300x50, 300x100, 375x50, 200x200, 250x250</p>-->
<!--              <p>Для ПК: 320x100, 300x500, 120x600, 200х300, 980x120, 980x90</p>-->
<!--              <p>Для планшетов: 768x1024, 1024x768, 640x360, 360x640</p>-->
<!--              <p>Рекомендуемые правила для создания HTML баннеров:</p>-->
<!--              <ul>-->
<!--                <li>Баннер должен быть представлен архивом из множества файлов: index.html и sprite.png (рекомендуется два и не более 100). В файле index.html допускаются только относительные ссылки на файлы-ресурсы.</li>-->
<!--                <li>Обязательно уменьшайте размер файлов sprite.png через сервис https://tinypng.com/</li>-->
<!--                <li>В index.html файле не допускается использование base64 представлений для изображений.</li>-->
<!--              </ul>-->
<!--              <p>Обработка в всех клик событий, вызывающих переход на сайт рекламодателя должна быть реализована строго через тег &lt;a href=””&gt;</p>-->
<!--            </q-card-section>-->
<!--          </q-card>-->
<!--        </q-expansion-item>-->
<!--        <q-expansion-item-->
<!--          expand-separator-->
<!--          label="Какие таргетинги есть?"-->
<!--          class="faq-section__accordion"-->
<!--          expand-icon="add"-->
<!--          expanded-icon="remove"-->
<!--          -->
<!--        >-->
<!--          <q-card>-->
<!--            <q-card-section>-->
<!--              <p>На данный момент есть возможность таргетироваться по:</p>-->
<!--              <ul>-->
<!--                <li>ГЕО</li>-->
<!--                <li>Устройствам (ПК/моб)</li>-->
<!--                <li>Браузерам</li>-->
<!--                <li>Операционным системам</li>-->
<!--                <li>Операторам связи</li>-->
<!--                <li>Аудиторным данным:</li>-->
<!--                <li>Соцдем (пол/возраст)</li>-->
<!--                <li>Интересы NativeLab - Собственные данные, основанные на потреблении контента</li>-->
<!--                <li>Сторонние данные: AmberData, Weborama</li>-->
<!--                <li>Ретаргетинг, Look-alike</li>-->
<!--              </ul>-->
<!--            </q-card-section>-->
<!--          </q-card>-->
<!--        </q-expansion-item>-->
<!--        <q-expansion-item-->
<!--          expand-separator-->
<!--          label="Какие счетчики поддерживает платформа?"-->
<!--          class="faq-section__accordion"-->
<!--          expand-icon="add"-->
<!--          expanded-icon="remove"-->
<!--          -->
<!--        >-->
<!--          <q-card>-->
<!--            <q-card-section>-->
<!--              Принимаем любые счетчики разных систем.-->
<!--            </q-card-section>-->
<!--          </q-card>-->
<!--        </q-expansion-item>-->
<!--      </q-list>-->
<!--      <q-btn-->
<!--        class="faq-section__main-btn main-btn main-btn&#45;&#45;blue main-btn&#45;&#45;wide"-->
<!--        data-aos="fade-up" data-aos-anchor-placement="top-center"-->
<!--        data-aos-duration="1000"-->
<!--        data-aos-once="true"-->
<!--        @click="router.push({name: 'registration'})">-->
<!--          Разместить рекламу-->
<!--      </q-btn>-->
<!--    </section>-->
<!--    <section class="features-section">-->
<!--      <div class="features-section__container container">-->
<!--        <h2 class="features-section__title title custom-font" >Собственный RTB движок и технологии</h2>-->
<!--        <p class="features-section__intro intro intro&#45;&#45;bold" >Особенности DMP</p>-->
<!--        <q-list class="features-section__list" >-->
<!--          <q-item class="features-section__item">-->
<!--            <p>-->
<!--              Собственный <b>сквозной идентификатор</b>, позволяющий платить за уникальный охват до 3х раз меньше-->
<!--            </p>-->
<!--          </q-item>-->
<!--          <q-item class="features-section__item">-->
<!--            <p>-->
<!--              Доступ к <b>данным Яндекса</b> для уточнения пола, возраста и интересов аудитории-->
<!--            </p>-->
<!--          </q-item>-->
<!--          <q-item class="features-section__item">-->
<!--            <p>-->
<!--              Модели <b>машинного обучения</b>, в том числе под СРА клиентов-->
<!--            </p>-->
<!--          </q-item>-->
<!--          <q-item class="features-section__item">-->
<!--            <p>-->
<!--              Возможность собрать <b>любой</b> кастомный сегмент-->
<!--            </p>-->
<!--          </q-item>-->
<!--          <q-item class="features-section__item">-->
<!--            <p>-->
<!--              <b>Интеграция</b> с другими DMP-->
<!--            </p>-->
<!--          </q-item>-->
<!--          <q-item class="features-section__item features-section__item&#45;&#45;big">-->
<!--            <p>-->
<!--              Привязка к <b>офлайн данным</b> позволяет-->
<!--            </p>-->
<!--            <p>-->
<!--              а) измерять эффективность каждого показа (влияние на конверсию)-->
<!--            </p>-->
<!--            <p>-->
<!--              б) обучать ML на фактических данных-->
<!--            </p>-->
<!--          </q-item>-->
<!--          <q-item class="features-section__item features-section__item&#45;&#45;last">-->
<!--            <p>-->
<!--              <b>Автообучаемые ML</b> для многих сфер бизнеса-->
<!--            </p>-->
<!--          </q-item>-->
<!--          <q-item class="features-section__item features-section__item&#45;&#45;last">-->
<!--            <p>-->
<!--              Проведение <b>опросов и замеров</b> OMI/ Tiboron-->
<!--            </p>-->
<!--          </q-item>-->
<!--        </q-list>-->
<!--      </div>-->
<!--    </section>-->
<!--    <section class="control-section">-->
<!--      <div class="control-section__container container">-->
<!--        <h2 class="control-section__title title title&#45;&#45;white custom-font" >Контроль за размещением рекламы</h2>-->
<!--        <p class="control-section__intro intro intro&#45;&#45;bold intro&#45;&#45;white" >Brand safety</p>-->
<!--        <div class="control-section__block">-->
<!--          <div class="control-section__block-item" >-->
<!--            <h3 >Защита бренда от фрода и ненужного контента</h3>-->
<!--            <q-list class="control-section__block-list">-->
<!--              <q-item class="control-section__block-list-item" >-->
<!--                <p>Стоимость размещения ниже, чем на других платформах</p>-->
<!--              </q-item>-->
<!--              <q-item class="control-section__block-list-item" >-->
<!--                <p>Применение контекстных фильтров</p>-->
<!--              </q-item>-->
<!--              <q-item class="control-section__block-list-item" >-->
<!--                <p>Black lists</p>-->
<!--              </q-item>-->
<!--              <q-item class="control-section__block-list-item" >-->
<!--                <p>Ручная оптимизация каждой рекламной кампании</p>-->
<!--              </q-item>-->
<!--              <q-item class="control-section__block-list-item" >-->
<!--                <p>Фильтрация по ключевым словам, контенту страницы</p>-->
<!--              </q-item>-->
<!--            </q-list>-->
<!--          </div>-->
<!--          <div class="control-section__block-item" >-->
<!--            <h3 >Высокое качество нашего трафика подтверждено</h3>-->
<!--            <div class="control-section__block-sign" >-->
<!--              <p>Антифрод А</p>-->
<!--            </div>-->
<!--            <p >Собственная система предотвращения фрода – Антифрод А</p>-->
<!--            <div class="control-section__block-imgs" >-->
<!--              <img class="control-section__block-img" src="~assets/main/weborama.jpg" srcset="~assets/main/weborama.jpg 1x, ~assets/main/weborama-2x.jpg 2x" alt="weborama">-->
<!--              <img class="control-section__block-img" src="~assets/main/adriver.jpg" srcset="~assets/main/adriver.jpg 1x, ~assets/main/adriver-2x.jpg 2x" alt="adriver">-->
<!--              <img class="control-section__block-img" src="~assets/main/sizmek.jpg" srcset="~assets/main/sizmek.jpg 1x, ~assets/main/sizmek-2x.jpg 2x" alt="sizmek">-->
<!--            </div>-->
<!--            <p >Применение верификаторов третьих сторон Weborama, AdRiver, Sizmek или других</p>-->
<!--          </div>-->
<!--        </div>-->
<!--        <q-btn-->
<!--          class="control-section__main-btn main-btn main-btn&#45;&#45;blue main-btn&#45;&#45;wide"-->
<!--          data-aos="fade-up"-->
<!--          data-aos-anchor-placement="top-center"-->
<!--          data-aos-duration="1000"-->
<!--          data-aos-once="true"-->
<!--          @click="router.push({name: 'registration'})"-->
<!--        >-->
<!--          Разместить рекламу-->
<!--        </q-btn>-->
<!--      </div>-->
<!--    </section>-->
<!--    <section class="partners-section container">-->
<!--      <h2 class="partners-section__title title custom-font" >Наши партнеры</h2>-->
<!--      <div >-->
<!--        <PartnersSlider/>-->
<!--      </div>-->
<!--    </section>-->
<!--    <section class="contacts-section">-->
<!--      <div class="contacts-section__container container">-->
<!--        <h2 class="contacts-section__title title custom-font" >Контакты</h2>-->
<!--        <div >-->
<!--          <ContactsSlider/>-->
<!--        </div>-->
<!--      </div>-->
<!--    </section>-->
<!--  </q-page>-->
</template>

<script setup lang="ts">
import { onMounted } from 'vue';
import ImgSlider from 'components/ImgSlider.vue';
import GeoSlider from 'components/GeoSlider.vue';
import TargetingSlider from 'components/TargetingSlider.vue';
import PartnersSlider from 'components/PartnersSlider.vue';
import ContactsSlider from 'components/ContactsSlider.vue';
// const AOS = require('aos');
// import {useRouter} from 'vue-router';

// const router = useRouter();

// onMounted(() => {
//   AOS.init();
// })
</script>
