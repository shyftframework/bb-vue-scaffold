<template lang="pug">
#app
  .uk-container-expand
    div(uk-sticky='sel-target: .uk-navbar-container; cls-active: uk-navbar-sticky; bottom: #transparent-sticky-navbar')
      nav.uk-navbar-container(uk-navbar='', style='position: relative; z-index: 980;')
        .uk-navbar-left
          ul.uk-navbar-nav
            li.uk-active
              a(href='#') Active
            li
              a(href='#') Parent
              .uk-navbar-dropdown
                ul.uk-nav.uk-navbar-dropdown-nav
                  li.uk-active
                    a(href='#') Active
                  li
                    a(href='#') Item
                  li
                    a(href='#') Item
            li
              a(href='#') Item
    img(src='./assets/logo.png')
    h1 {{ msg }}
    h2 Essentials
    ul
      li
        a(href='https://vuejs.org', target='_blank') Core Docs
      li
        a(href='https://forum.vuejs.org', target='_blank') Forum
      li
        a(href='https://gitter.im/vuejs/vue', target='_blank') Gitter Chat
      li
        a(href='https://twitter.com/vuejs', target='_blank') Twitter
    h2 The Vue Ecosystem
    ul
      li
        a(href='http://router.vuejs.org/', target='_blank') vue-router
      li
        a(href='http://vuex.vuejs.org/', target='_blank') vuex
      li
        a(href='http://vue-loader.vuejs.org/', target='_blank') vue-loader
      li
        a(href='https://github.com/vuejs/awesome-vue', target='_blank') awesome-vue
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to your Backbase Vue.js Widget!'
    }
  }
}
</script>

<style lang="scss">
// import uikit sass files
@import "assets/scss/variables.scss";
@import "assets/scss/uikit.scss";
@import "assets/scss/components/_import.scss";

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

h1, h2 {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
