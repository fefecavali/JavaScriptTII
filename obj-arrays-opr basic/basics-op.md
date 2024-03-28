# 1B04 - Operadores Básicos

- **Explicação textual do conceito**
- **Exemplos com códigos**
- **Exercício(s) para fixação**
  
#
## Conceito
Os operadores básicos em JavaScript são usados para realizar operações matemáticas, comparações, atribuições, etc.
O JavaScript possui tanto operadores binários quanto unários e um operador ternário, o operador condicional. 

## Exemplos de códigos

### Operadores de atribuição

```javascript
let x = 16;
x -= 2; // x é agora 14 (subtração e atribuição)
```

### Operadores de comparação

```javascript
let a = 5;
let b = '5';

console.log(a == b); // true (coerção de tipo)
console.log(a === b); // false (sem coerção de tipo)
```
### Operadores aritméticos

```javascript
// Adição e subtracao
let soma = 2 + 3; //  5
let diferenca = 5 - 3; // 2

// Multiplicação e divisao
let produto = 4 * 2; // 8
let quociente = 10 / 2; // 5

// Módulo
let resto = 10 % 3; // resto é 1 
// Exponenciação
let potencia = 2 ** 3; // 8 
```
### Operadores lógicos

```javascript
let idade = 25;
let salario = 3000;

console.log(idade >= 18 && salario > 2000); // true (ambas as condições são verdadeiras)
console.log(idade < 18 || salario < 1500); // false (nenhuma das condições é verdadeira)
console.log(!(idade > 30)); // true (negação da condição)
```
## Exercício(s) para fixação
**Crie um programa que realize operações aritméticas básicas em dois números fornecidos pelo usuário e exiba os resultados.**

```javascript
// prompt == input
let numero1 = parseFloat(prompt("Digite o primeiro número:"));
let numero2 = parseFloat(prompt("Digite o segundo número:"));


let soma = numero1 + numero2;
let subtracao = numero1 - numero2;
let multiplicacao = numero1 * numero2;
let divisao = numero1 / numero2;

// Exibir os resultados
console.log(`Soma: ${soma}`);
console.log(`Subtração: ${subtracao}`);
console.log(`Multiplicação: ${multiplicacao}`);
console.log(`Divisão: ${divisao}`);
```