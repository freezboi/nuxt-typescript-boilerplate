<template>
  <div>
    <logo />
    <h1>Hello world!!</h1>
    <p>{{ authorName }}</p>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';
import Logo from '~/components/Logo.vue';

@Component({
  components: {
    Logo
  }
})
export default class HelloComponent extends Vue {
  authorName: string = 'chihoon';
}
</script>
