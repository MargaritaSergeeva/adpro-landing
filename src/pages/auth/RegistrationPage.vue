<template>
  <div class="registration-page">
    <h1 class="registration-page__title guest-title custom-font">Registration</h1>
    <q-form class="registration-page__form registration-form" @submit.prevent.stop="onSubmit">
      <div class="registration-form__form-wrapper">
        <div class="registration-form__group">
          <label class="label">Company Name</label>
          <q-input
            ref="organizationNameInputRef"
            v-model="registrationData.organization_name"
            dense
            square
            borderless
            bottom-slots
            lazy-rules
            class="input"
            :rules="[rules.required, rules.minLen(3), rules.maxLen(60)]"
          />
        </div>
        <div class="registration-form__group">
          <label class="label">Password</label>
          <q-input
            ref="passwordInputRef"
            v-model="registrationData.password"
            :type="isPassword ? 'password' : 'text'"
            lazy-rules
            dense
            square
            borderless
            class="input"
            :rules="[rules.required, rules.minLen(8)]"
            @keydown.space.prevent
          >
            <template #append>
              <q-icon
                class="cursor-pointer"
                :style="{color: isPassword ? '#C4C4C4' : '#5D5FEF'}"
                @click="isPassword = !isPassword"
              >
                <div v-if="!isPassword" class="login-form__eye-visible">
                  <svg width="16" height="16" viewBox="0 0 16 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path
                      d="M11.9603 9.95985C10.8207 10.8285 9.43306 11.3098 8.00033 11.3332C3.33366 11.3332 0.666992 5.99985 0.666992 5.99985C1.49625 4.45445 2.64642 3.10426 4.04033 2.03985M6.60033 0.826521C7.05921 0.719107 7.52904 0.665413 8.00033 0.666521C12.667 0.666521 15.3337 5.99985 15.3337 5.99985C14.929 6.75693 14.4464 7.46968 13.8937 8.12652M9.41366 7.41319C9.23056 7.60969 9.00976 7.76729 8.76443 7.8766C8.5191 7.98591 8.25426 8.04469 7.98572 8.04943C7.71718 8.05417 7.45043 8.00477 7.2014 7.90418C6.95236 7.80359 6.72614 7.65387 6.53622 7.46396C6.34631 7.27404 6.19659 7.04782 6.096 6.79878C5.99541 6.54975 5.94601 6.283 5.95075 6.01446C5.95549 5.74592 6.01426 5.48108 6.12358 5.23575C6.23289 4.99042 6.39049 4.76962 6.58699 4.58652"
                      stroke="#999999" stroke-width="1.33333" stroke-linecap="round" stroke-linejoin="round"/>
                  </svg>
                </div>
                <div v-else class="login-form__eye-invisible">
                  <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path
                      d="M11.9603 11.9599C10.8207 12.8285 9.43306 13.3098 8.00033 13.3332C3.33366 13.3332 0.666992 7.99985 0.666992 7.99985C1.49625 6.45445 2.64642 5.10426 4.04033 4.03985M6.60033 2.82652C7.05921 2.71911 7.52904 2.66541 8.00033 2.66652C12.667 2.66652 15.3337 7.99985 15.3337 7.99985C14.929 8.75693 14.4464 9.46968 13.8937 10.1265M9.41366 9.41319C9.23056 9.60969 9.00976 9.76729 8.76443 9.8766C8.5191 9.98591 8.25426 10.0447 7.98572 10.0494C7.71718 10.0542 7.45043 10.0048 7.2014 9.90418C6.95236 9.80359 6.72614 9.65387 6.53622 9.46396C6.34631 9.27404 6.19659 9.04782 6.096 8.79878C5.99541 8.54975 5.94601 8.283 5.95075 8.01446C5.95549 7.74592 6.01426 7.48108 6.12358 7.23575C6.23289 6.99042 6.39049 6.76962 6.58699 6.58652"
                      stroke="#999999" stroke-width="1.33333" stroke-linecap="round" stroke-linejoin="round"/>
                    <path d="M0.666992 0.666504L15.3337 15.3332" stroke="#999999" stroke-width="1.33333"
                          stroke-linecap="round" stroke-linejoin="round"/>
                  </svg>
                </div>
              </q-icon>
            </template>
          </q-input>
        </div>
        <div class="registration-form__group">
          <label class="label">Business email</label>
          <q-input
            ref="emailInputRef"
            v-model="registrationData.email"
            type="email"
            dense
            square
            borderless
            class="input"
            :rules="[rules.required, rules.email]"
            @keydown.space.prevent
          />
        </div>
        <div class="registration-form__group">
          <label class="label">Telephone number</label>
          <q-input
            ref="phoneInputRef"
            v-model="registrationData.phone"
            dense
            square
            borderless
            bottom-slots
            lazy-rules
            type="number"
            :rules="[rules.required]"
            class="input"
          />
        </div>
      </div>

        <q-btn class="registration-form__main-btn main-btn main-btn--green main-btn--wide" type="submit">To Register</q-btn>

        <div class="registration-form__checkbox">
        <q-checkbox
          v-model="registrationData.is_privacy_policy_agreed"
          class="checkbox"
          dense
          checked-icon="done"
        >
          <template #default>
            Accept <router-link to="privacy-policy">privacy policy</router-link>
          </template>
        </q-checkbox>
      </div>

      <q-inner-loading
        :showing="processing"
        label-class="text-teal"
        label-style="font-size: 1.1em"/>
    </q-form>
  </div>
</template>


<script lang="ts" setup>
import {ref, computed, reactive} from 'vue';
import {useAuth} from '@websanova/vue-auth';
import axios from 'axios';
import {Validate} from 'src/common/validateErrors';

interface RegistrationDataInterface {
  organization_name: string,
  phone: string,
  email: string,
  password: string,
  is_privacy_policy_agreed: boolean,
}

interface FormErrorsInterface {
  email: string;
  password: string,
  phone: string,
}


const auth = useAuth();
const processing = ref(false);
const isPassword = ref(true);

const organizationNameInputRef = ref();
const emailInputRef = ref()
const phoneInputRef = ref()
const passwordInputRef = ref();

const registrationData = reactive<RegistrationDataInterface>({
  organization_name: '',
  phone: '',
  email: '',
  password: '',
  is_privacy_policy_agreed: true,
});

const formErrors = ref<FormErrorsInterface>({
  email: '',
  password: '',
  phone: '',
})

async function onSubmit() {
  if (!checkValidate.value) {
    return
  }
  processing.value = true;
  await auth.register({
    data: {...registrationData},
    autoLogin: true,
    staySignedIn: true,
    fetchUser: true
  }).then(() => {
    console.log(registrationData)
    auth.ready();
  }).catch((err) => {
    processing.value = false;
    if (axios.isAxiosError(err)) {
      if (err.response?.status === 422) {
        new Validate(err.response?.data, formErrors.value)
      }
    }
  }).finally(() => {
    processing.value = false;
  })
}

const checkValidate = computed(() => (...inputs: any[]) => {
  console.log(inputs)
  return inputs.reduce((isValid = true, input) => {
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
