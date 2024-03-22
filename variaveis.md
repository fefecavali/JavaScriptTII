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
# Tipos primitivos
Em Javascript os tipos primitivos são imutáveis.Existem 6 tipos primitivos em JavaScript, eles são: 

- **Number**: Representa valores numéricos, sejam inteiros ou de ponto flutuante. 

- **String**: Representa uma sequência de caracteres.

- **Booleano (Boolean)**: Representa um valor lógico true ou false ;

- **Undefined**: Representa uma variável que foi declarada, mas não atribuída com um valor;

- **Null**: Representa um valor vazio ou nulo;

- **Symbol**: Representa um tipo de dado único e imutável, muitas vezes usado como identificadores únicos de propriedades de objetos.

### Exemplos: 
```javascript

let pi = 3.14 //ex number

let message = ' Hello World!'  //ex string

let booleano = true; 
let a = undefined; //ex tipo indefinido

let nulo = null ;
let simbolo = Symbol('descricao');


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

#
# Exercícios Variáveis  e tipos primitivos em JavaScript

```javaScript
// Declare duas variáveis as quais serão do tipo String e junte-as 

//exemplo de solução -->

let nome1 = 'Fernanda'
let sobrenome = 'Cavali'

let nomeCompleto = nome1+ " " + sobrenome;

console.log("Nome completo:", nomeCompleto);
```

```javaScript

// Declare duas variáveis do tipo number e calcule o resultado da sua solução. 

//exemplo de solução -->

let num1 = 15 ;
let num2 = 3.15 ;

let resultado = num1/num2 ;


console.log("Divisão:", resultado);

```
```javaScript
// Declare uma variável indefinida e outra nula

//solução -->

let variavelIndef = undefined
let variavelNula = null

```
```javascript
// Crie um símbolo com uma descrição personalizada. Em seguida, declare um objeto com uma propriedade cuja chave seja o símbolo criado e imprima o objeto no console.

//solução -->

let descricaoSimbolo = "descricao_personalizada";
let meuSimbolo = Symbol(descricaoSimbolo);
let objeto = {};

objeto[meuSimbolo] = "Valor do símbolo";

console.log(objeto);
```

```javascript
// Declare uma variável e atribua a ela um valor numérico. Em seguida, declare uma variável temperatura e atribua a ela o valor true se a temperatura for menor que 15 graus, e false caso contrário. 

//solução -->

let valor = 10;
let temperatura = valor < 15;

console.log("Frio:", temperatura);


```






## by Fernanda Moreira Cavali