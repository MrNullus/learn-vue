# Inputs e Data Binding

O Vue como outros frameworks, trabalha com o conceito de data bings (amarrar ou vincular dados no português).

Inclusive ele consegue tratar essa questão de forma mais fácil

> Nem preciso falar que tudo é inputs, a computação não existe sem inputs

## Fazendo

- O `v-model` indica para o Vue que esse campo será assistido pelo Vue, ou seja, o valor desse campo será manipulado

> Ou seja, é uma diretiva do Vue para indicar que um campo faz parte do modelo, ou seja, o valor desse campo será
> manipulado

```html
<input type="text" v-model="input_name" placeholder="Digite seu nome">
```

- Adicionando diretiva de click `v-on-click` para receber e assistir uma função que será executada assim que houver
  click no elemento:

````
<input type="submit" value="Enviar" v-on:click="submitForm">
````

### Entendendo algumas coisas

O atributos `methods` é onde definiremos todos os metodos do App, onde ficaram todas as funções que o Vue vai ter
acesso:

```js
methods: {
    submitForm(e) {
        e.preventDefault()
        console.log(this.input_name);

        this.name = this.input_name;
    }
}
```
