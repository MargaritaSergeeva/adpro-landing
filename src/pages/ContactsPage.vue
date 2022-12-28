<template>
  <q-page class="contacts-page">
    <section class="main-contacts-section container">
      <div class="main-contacts-section__item">
        <h1 class="custom-font main-contacts-section__title main-title">Contacts</h1>
        <div class="main-contacts-section__map map-block">
          <div class="map-block__map">
            <img src="~assets/contacts/map.jpg" alt="map">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d815.404147255466!2d33.357495829225954!3d35.16618169510296!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x14de1757a757762f%3A0xbb1e41a00906969!2sThemistokli%20Dervi%2017-19-HOUSE%2C%202nd%20floor%201066%2C%20Nicosia%2C%20%D0%9A%D0%B8%D0%BF%D1%80!5e0!3m2!1sru!2sru!4v1672241081109!5m2!1sru!2sru" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
          </div>
          <p>Themistokli Dervi, 17-19 THE CITY HOUSE, 2nd floor 1066, Nicosia, Cyprus</p>
        </div>
      </div>
      <div class="main-contacts-section__item main-contacts-section__item--big">
        <h2>Any questions left? We are ready to help.</h2>
        <p>To receive a presentation, cases or you have questions, fill out the form:</p>
        <q-form class="main-contacts-section__form contacts-form" @submit="submit">
          <div class="contacts-form__group">
            <label for="name" class="contacts-form__label label">First and last name</label>
            <q-input
              ref="nameInputRef"
              v-model="contactsFormData.name"
              id="name"
              class="contacts-form__input input"
              square
              borderless
              :rules="[rules.required, rules.minLen(3), rules.maxLen(50)]"
            ></q-input>
          </div>
          <div class="contacts-form__group-wrapper">
            <div class="contacts-form__group contacts-form__group--big">
              <label for="email" class="contacts-form__label label">Email</label>
              <q-input
                ref="emailInputRef"
                v-model="contactsFormData.email"
                id="email"
                class="contacts-form__input input"
                square
                borderless
                :rules="[rules.required, rules.email]"
              ></q-input>
            </div>
            <div class="contacts-form__group">
              <label for="phone" class="contacts-form__label label">Phone</label>
              <q-input
                ref="phoneInputRef"
                v-model="contactsFormData.phone"
                id="phone"
                class="contacts-form__input input"
                square
                borderless
                type="number"
                :rules="[rules.required]"
              ></q-input>
            </div>
          </div>
          <div class="contacts-form__group">
            <label for="company" class="contacts-form__label label">Company name</label>
            <q-input
              ref="nameCompanyInputRef"
              v-model="contactsFormData.company"
              id="company"
              class="contacts-form__input input"
              square
              borderless
              :rules="[rules.required, rules.minLen(3), rules.maxLen(50)]"
            ></q-input>
          </div>
          <div class="contacts-form__group">
            <label for="text" class="contacts-form__label label">Your message</label>
            <q-input
              v-model="contactsFormData.text"
              id="text"
              class="contacts-form__input input input--textarea"
              square
              borderless
              type="textarea"
            ></q-input>
          </div>
          <q-btn class="contacts-form__main-btn main-btn main-btn--green main-btn--wide" type="submit">Send</q-btn>
        </q-form>
      </div>
    </section>
  </q-page>
</template>

<script setup lang="ts">
import {computed, ref} from 'vue';

interface contactsFormData {
  name: string,
  email: string,
  phone: string,
  company: string,
  text: string,
}

const contactsFormData = ref<contactsFormData>({
  name: '',
  email: '',
  phone: '',
  company: '',
  text: '',
});

const nameInputRef = ref();
const emailInputRef = ref();
const phoneInputRef = ref();
const nameCompanyInputRef = ref();

const submit = () => {
  if (!checkValidate.value) {
    return;
  }
};

const checkValidate = computed(() => {
  const formInputs = [
    nameInputRef.value,
    emailInputRef.value,
    phoneInputRef.value,
    nameCompanyInputRef.value,
  ];

  return formInputs.reduce((isValid = true, input) => {
    const isValidInput = input.validate();
    if (!isValidInput) isValid = isValidInput;
    return isValid;
  }, []);
});

const rules = {
  required: (v: boolean | undefined) => !!v || 'Поле обязательно для заполнения',
  minLen: (minLen: number) => (v: string) => {
    return v.length >= minLen || `Минимум ${minLen} символов`;
  },
  maxLen: (maxLen: number) => (v: string) => {
    return v.length <= maxLen || `Максимум ${maxLen} символов`;
  },
  email: (v: string) => {
    const emailPattern = /.+@.+\..+$/;
    return emailPattern.test(v) || 'Неверный формат email';
  },
};
</script>
