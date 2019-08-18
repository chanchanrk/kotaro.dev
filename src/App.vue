<template>
  <div id="app">
    <div id="contents">
      <Links />
    </div>
  </div>
</template>

<script>
import Links from './components/Links.vue'

export default {
  name: 'app',
  components: {
    Links
  }
}
</script>

<style>
html {
  height:100%;
}
body {
  height:100%;
}
#app {
  display:table;
  width:100%;
  height:100%;
}
#contents {
  display:table-cell;
  vertical-align:middle;
  text-align:center;
}
#contents ul {
  list-style: none;
  display:inline-block;
}
#contents ul li {
  text-align:left;
}
</style>
