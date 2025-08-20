<template>
  <div class="app">
    <Header />
    <main class="content">
      <router-view />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  components: { Header, Footer }
}
</script>

<style>
/* Layout para empurrar o footer pro final da página */
.app {
  min-height: 100vh;           /* pega a altura total da tela */
  display: flex;
  flex-direction: column;      /* empilha header, conteúdo e footer */
}

.content {
  flex: 1;                     /* ocupa o espaço “vago” entre header e footer */
}
</style>
