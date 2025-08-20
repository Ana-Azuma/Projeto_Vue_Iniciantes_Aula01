<template>
  <header class="site-header">
    <h1>Agência de Viagem</h1>
    <nav>
      <router-link to="/">Início</router-link>
      <router-link to="/about">Sobre</router-link>
      <router-link to="/services">Serviços</router-link>
    </nav>
  </header>
</template>

<style scoped>
.site-header {
  background: linear-gradient(135deg, #007399, #00c6ff);
  padding: 1rem;
  text-align: center;
  color: white;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
}

.site-header h1 {
  margin: 0 0 0.5rem 0;
}

nav a {
  color: white;
  margin: 0 1rem;
  text-decoration: none;
  font-weight: bold;
}

nav a:hover {
  text-decoration: underline;
}
</style>
