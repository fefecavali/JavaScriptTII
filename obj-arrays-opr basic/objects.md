# 1B04 - Estudo Objetos

- **Explicação textual do conceito**
- **Exemplos com códigos**
- **Exercício(s) para fixação**
#
## Conceito
Objetos são entidades independentes, com propriedades (associação entre um nome (ou chave) e um valor) e tipos.
Uma propriedade de um objeto pode ser explicada como uma variável que é ligada ao objeto ou pode ser uma função, que é então considerada um método do objeto. 

## Exemplos de códigos

```javascript

var carro = {
  cor: "vermelho",
  rodas: 4,
  motor: { cilindros: 4, tamanho: 2.2 },
};

console.log(carro.cor); // Saída: vermelho

//usando função construtora
function Carro(marca, modelo, ano) {
  this.marca = marca;
  this.modelo = modelo;
  this.ano = ano;
}
//criando 3 objetos do tipo Carro
var meucarro = new Carro("Eagle", "Talon TSi", 1993);
var carroDeKen = new Carro("Nissan", "300ZX", 1992);
var carroDeVPG = new Carro("Mazda", "Miata", 1990);
```


## Exercício(s) para fixação

**Crie um programa em JavaScript que represente os sabores de sorvete disponíveis em uma sorveteria, cada um com seu tipo (se é cremoso, frutado, etc.). Em seguida, exiba essas informações no console.**

```javascript
//Definindo objeto
let sorveteria = {
    sabores: [
        { nome: "Morango", tipo: "Frutado" },
        { nome: "Chocolate", tipo: "Cremoso" },
        { nome: "Limão", tipo: "Frutado" },
        { nome: "Baunilha", tipo: "Cremoso" },
        { nome: "Manga", tipo: "Frutado" }
    ]
};

// Função para exibir as informações dos sabores de sorvete
function exibir(sorveteria) {
    console.log("Sorveteria - Sabores Disponíveis:");
    sorveteria.sabores.forEach((sabor, index) => {
        console.log(`Sabor ${index + 1}: ${sabor.nome} (${sabor.tipo})`);
    });
}

exibir(sorveteria);

```
