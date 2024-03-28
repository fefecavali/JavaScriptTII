# 1B04 -  Arrays 

- **Explicação textual do conceito**
- **Exemplos com códigos**
- **Exercício(s) para fixação**
  
#
## Conceito

Arrays são objetos de alto nível semelhantes a listas. Podendo ser construídas com o objeto `Array`.
Elas permitem que armazenemos multiplos valores dentro de uma variável e viabiliza a manipulação e interação com estes.


## Exemplos de códigos

**- Método push insere elementos na array ;**

**- Método pop deleta ultimo elemento ;**

**- Método indexOf retorna indice do primeiro elemento escolhido que aparecer ;**
```javascript

var frutas = [];
frutas.push("banana", "maça", "pêssego", "abacaxi");

console.log(frutas.length); // 3

frutas.pop();

console.log(frutas); // Saída: ["banana", "maça", "pêssego"]

console.log(frutas.indexOf("maça")); // Saída: 1
```


## Exercício(s) para fixação

**Escreva uma função em JavaScript que receba uma lista de nomes e retorne os nomes em ordem alfabética.**

- método `sort` ordena
```javascript

function ordenarNomes(nomes) {
    nomes.sort();
    return nomes;
}

const nomes = ["Fernanda", "Roberto", "Amanda", "Matheus", "Valmir"];

const nomesOrdenados = ordenarNomes(nomes);

console.log(nomesOrdenados);
```