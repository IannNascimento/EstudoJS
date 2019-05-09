
# Variáveis e tipo de dados

## Variáveis

### Conceito de variáveis 
#### Variáveis ​​JavaScript são contêineres para armazenar valores de dados.
A declaração de uma variável no JavaScript é representada pela palavra **var**

Neste exemplo, **idade**, **nome** e **casado** são variáveis

```
var idade = 24;
var nome = "Iann";
var casado = false;
```
Do exemplo acima, você pode esperar:

**idade** armazena o valor 24
**nome** armazena o valor Iann
**casado** armazena o valor false

>  Se o valor não for especificado, essa variável será nula (sem
> valor), até que isso aconteça.

### Tipos de variáveis
* #### Variáveis comum
As variáveis podem ser declaradas de diferentes maneiras, mantendo o mesmo resultado

Exemplo 1 - Separada uma por linha já atribuindo o valor
```
var  idade = 24;
var  nome = "Iann";
var  casado = false;
```
Exemplo 2 - Separada uma por linha, atribuindo o valor ao decorrer da programação
```
var  idade;
var  nome ;
var  casado;

idade = 24;
nome = "Iann";
casado = false;
```
Exemplo 3 - todos em uma linha separados por virgula "," já atribuindo o valor
```
var  idade = 24, nome = "Iann", casado = false;
```
Exemplo 4 - todos em uma linha separados por virgula ",", atribuindo o valor ao decorrer da programação
```
var  idade, nome, casado;

idade = 24;
nome = "Iann";
casado = false;
```
 * #### Arrays
 Array é uma variável multidimensional, que pode ser usada para armazenar vários valores em uma única variável
  Exemplo:
```
var dados = ["nome1", "nome2", "nome3"]
```

Do exemplo acima, você pode esperar:
dados recebe o valor de **nome1**, **nome2** e **nome3**

Como array recebe vários valores, os elementos são acessados usando índices numéricos (a partir de 0).

Esta declaração acessa o valor do **primeiro** elemento em **dados**
```
<!DOCTYPE html>
<html lang="pt-br">
<head>

<meta  charset="utf-8">
<title> Array</title>

</head>
<body>

<h1>JavaScript Arrays</h1>

<p id="nomeEscolhido"></p>

<script>
var dados = ["nome1", "nome2", "nome3"];
document.getElementById("nomeEscolhido").innerHTML = dados [0];
</script>

</body>
</html>
```
* #### Objeto
Objeto é um tipo de variável que podem conter muitos valores 
```
var pessoa = {nome: "Iann, idade: 24, casado: false};
```
Os valores são gravados como **nome:** pares de **valores** (nome e valor separados por dois pontos)

> Objetos JavaScript são contêineres para **valores nomeados** chamados **propriedades** ou **métodos**.
* ##### Propriedades do Objeto
O **nome:** pares de **valores** em objetos são chamados de **propriedades** :
|Propriedade|Valor da propriedade|
|--|--|
|nome|Iann|
|idade |24|
|casado|false|
Para acessar as propriedades dos objetos, usasse os nomes das propriedades

> Diferente de array, as propriedades não são ordenadas por números (0,
> 1, 2)

Há duas maneiras para acessar as propriedades dos objetos:
```
var pessoa = {nome: "Iann, idade: 24, casado: false};
document.getElementById("demo").innerHTML = pessoa.nome;
```
Ou
```
var pessoa = {nome: "Iann, idade: 24, casado: false};
document.getElementById("demo").innerHTML = pessoa["nome"];
```
* ##### Métodos de objeto
Objetos também podem ter **métodos** . Métodos são **ações** que podem ser executadas em objetos.
Os métodos são armazenados em propriedades como **definições de função** .
```
var pessoa = {
	nome: "Iann",
	sobrenome: "Nascimento",
	idade: 24,
	casado: false,
	nomeCompleto: function(){
		return this.nome + " " + this.sobrenome;
		}
};

console.log(pessoa.nomeCompleto())
```
|Propriedade|Valor da propriedade|
|--|--|
|nome|Iann|
|sobrenome|Nascimento|
|nomeCompleto|function ( ) {return this.nome + " " + this.sobrenome}|
|idade |24|
|casado|false|

> Um método é uma função armazenada como uma propriedade.

## Tipos de dados
Os tipos de dados são os "tipos de valores" recebidos pelas propriedades das variáveis, como por exemplo:
*  **Strings**

> Conteúdo de textos, obrigatoriamente dentro de aspas simples ou dupla. 

*  **Numbers**

> Conteúdo numérico (0, 1, 2, 3, 4, 5, 6, 7, 8, 9).
 * **Booleans**
> Falso ou verdadeiro (false, true).
 *  **Arrays**
 
 *  **Objects**
 
 * **Undefined**
> Tipo indefinido
 *  **Empty Values**
> Valores vazios - Um valor vazio não tem nada a ver com `undefined`.
> Uma string vazia tem um valor legal e um tipo.
 * **Null**
 
 *  **Function**
