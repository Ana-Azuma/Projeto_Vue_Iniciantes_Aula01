# Vue + Vite

Siste de agência de viajens.

Qual a função do main.js? 
O main.js é o ponto de entrada da aplicação Vue. É nele que você cria a instância da sua aplicação, registra plugins (como Vue Router, Vuex/Pinia) e finalmente monta a aplicação no HTML.

O que é o App.vue? 
O App.vue é o componente raiz da aplicação. Todos os outros componentes, rotas e views normalmente são “filhos” dele. Serve como layout global, podendo conter cabeçalhos, menus, rodapés etc.

Para que servem os arquivos views? 
As views são componentes grandes que representam páginas da aplicação.
Por exemplo:
Home.vue → página inicial
About.vue → página “sobre”
Eles ficam na pasta views e normalmente são usados como destino das rotas.

Como o VUE Router usa as views? 
No arquivo router/index.js ou router.js, você define as rotas e indica qual view será carregada. Quando o usuário acessa /about, o Vue Router injeta o componente About.vue dentro do <router-view /> do App.vue. Isso mantém a aplicação SPA (Single Page Application), sem recarregar a página.

Como que faz app.mount('#app')?
Essa linha fala para o Vue: “exiba a aplicação no elemento HTML que tem id app”.
No seu index.html, você teria algo assim: <div id="app"></div>
Basicamente, o Vue substitui o conteúdo desse div pelo template do App.vue e tudo que for renderizado dentro dele.
