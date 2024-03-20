# Variáveis  e tipos primitivos em JavaScript

## Declaração de variáveis

A declaração de variávies em JavaScript é feita de três formas :

- **var** : Forma original ( não muito utilizada ). Variáveis declaradas com *'var'* têm escopo de função ou global ;
  
- **let** : Tem escopo de bloco. Diferente do 'var', quando usamos o *'let'* não podemos acessar o valor antes de sua declaração no código ;
  
- **const** : Usada para indicar constantes em escopo de bloco. O valor da constante não pode ser alterado após a inicialização .
  
**Exemplo :**
```javascript

var pi = 3.14 ;

let nome = 'Fernanda' ;

const ano = 2024 ;


```


#
# Escopo
O escopo é responsável pela visibilidade e acessibilidade de variáveis, funções e objetos dentro de um programa. 
Existem três principais tipos: escopo global, escopo local e escopo de bloco


### Global

As variáveis declaradas fora de qualquer função têm escopo global, o que significa que elas podem ser acessadas de qualquer lugar no código.

Exemplo: 

```javascript
var nome = 'fer'
function exemploGlobal() {
    console.log(nome); 
}

exemploGlobal(); 

```

### Bloco

Variáveis declaradas com let e const têm escopo de bloco, o que significa que elas só podem ser acessadas dentro do bloco em que foram declaradas.

```Javascript
function exemploBloco() {
    if (true) {
        let variavelBloco = 'Hello';
        console.log(variavelBloco); 
    }
    console.log(variavelBloco);  //erro pq a variavel não esta acessivel aqui 

exemploBloco();
```

### Local
As variáveis declaradas dentro de uma função têm escopo local e só podem ser acessadas dentro dessa função.

```Javascript
function exemploLocal() {
    var variavelLocal = 20;
    console.log(variavelLocal); // Acesso à variável local
}

exemploLocal(); // Saída: 20
console.log(variavelLocal); // erro, variavel não está acessível aqui.

```

