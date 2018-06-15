<template>
  <div class="theme-container">
    <div class="content">
      <h1>404</h1>
      <blockquote>{{ getMsg() }}</blockquote>
      <router-link to="/">Ramène moi à la maison.</router-link>
    </div>
  </div>
</template>

<script>
const msgs = [
  `Il n'y a rien ici.`,
  `Comment est-on arrivé là ?`,
  `C'est une Quatre-Zéro-Quatre !`,
  `On dirait qu'on a un lien mort...`
]

export default {
  methods: {
    getMsg () {
      return msgs[Math.floor(Math.random() * msgs.length)]
    }
  }
}
</script>
