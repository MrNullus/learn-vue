# Instalação
* Podemos instalar por **CDN**, ou seja, um link dentro do HTML
  * Algumas funcionalidades podem não existir ou funcionar bem, usando CDN
* Assim como podemos usar a **CLI** -> a forma mais recomendada


## CDN
- Anexar esse link, que pode se achar na documentação oficial do Vue, dentro do html:
```html
<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
```

- Assim teremos:
````html
<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>

<div id="app">{{ message }}</div>

<script>
  const { createApp, ref } = Vue

  // construir o app
  createApp({
    setup() {
      const message = ref('Hello vue!')
      return {
        message
      }
    }
  }).mount('#app') // definir onde o app será montado
</script>
````

## Via CLI

> :exclamation: Pre-requisitos: **Install Node.js version 18.3 or higher**

- Rodar o comando:
````bash
npm create vue@latest
````
- Depois disso, caso houve sucesso basta:
```bash
cd <your-project-name> // ir para seu projeto vue criado
npm install // instalar as dependencias
npm run dev // rodar o projeto vue criado 
```

