<template>
  <div class="links">
    <ul class="link-ul">
      <li><img id="icon" src="@/assets/icon.jpg"/></li>
      <li>kotaro</li>
      <li v-for="link in links" v-bind:key="link.service">
          {{ link.service }} : <a v-bind:href="link.url">{{ link.name }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
import links from '../assets/links.json'
export default {
  name: 'Links',
  data: function() {
    return {
      links: links
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#icon {
  width: 100px;
  height: 100px;
}
</style>
