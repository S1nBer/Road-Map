<template>
  <LoginForm />
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HelloWorld from './components/HelloWorld.vue';
import LoginForm from './components/LoginForm.vue';

@Options({
  components: {
    HelloWorld,
    LoginForm,
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
body {
    margin: 0;
}

#app {
    width: 100vw;
    height: 100vh;
}
</style>
