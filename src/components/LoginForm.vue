<template>
  <div class="loginForm">
    <div class="form"></div>
    <div class="background">
      <img
        class="background-img"
        src="https://img2.akspic.ru/previews/1/6/7/3/4/143761/143761-zakat-apelsin-voshod_solnca-gorizont-gornyj_relef-x750.jpg"
        alt="background"
      />
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
  props: {
    msg: String,
  },
})
export default class LoginForm extends Vue {
  msg!: string;
}
</script>

<style scoped lang="scss">
.loginForm {
  width: 100%;
  height: 100%;
  display: flex;

  .form {
    width: 55%;
  }

  .background {
    width: 45%;
    position: relative;
    overflow: hidden;

    .background-img {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}
</style>
