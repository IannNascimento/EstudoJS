# Conceitos JavaScript

## O que é JavaScript?

### JavaScript é uma linguagem de programação client-side
Não é executado no servidor e sim no cliente (navegadores)

### Ela é utilizada para controlar o HTML e o CSS para manipular comportamentos na página, como
* Abrir e fechar janelas do navegador
```
Abrir uma nova aba ou fechar alguma aberta
```
* Avançar e retroceder
```
Trocar de páginas, fotos de Slides, etc
```
* Ocultar ou mostrar elementos da página
```
Ocultar um submenu e fazer ele aparecer após uma ação 
```
* Alterar o conteúdo HTML da página
```
Adicionar ou remover textos de um determinado elemento (sem fazer alteração no HTML)
```
* Alterar estilos CSS da página
```
 Alterar cor de um determinado botão após uma ação
```
## Vantagens linguagem JavaScript
* Não há necessidade de processamento de seu servidor, isso dar ao usuário uma resposta mais rápida
* Praticidade - Precisasse apenas de um editor de códigos (Ex: Visual Studio Code) para escrever os códigos e um navegador para executar os códigos (sem necessidade de servidores).

## Desvantagens linguagem JavaScript

* Como todo o código JavaScript está no próprio navegador, o usuário pode ver o código e pode também, através da utilização de alguns programas, manipular o código. Isso faz com que as linguagens client-side sejam inseguras para fazer coisas como acessar um banco de dados
* Como linguagem JavaScript é client Side, ele depende da compatibilidade de cada navegador, isso acaba gerando dúvida se o JS vai ou não rodar no computador do cliente. Hoje com navegadores mais modernos (google chrome, mozila, opera, etc) não existem muitos problemas.

## Colocando JavaScript no HTML
### * O códigos JavaScript escrito no HTML, deve ficar obrigatoriamente dentro de uma tag chamada SCRIPT (<Script></Script>) podendo ficar dentro das tags head ou body. Porém o correto (padrão) é colocar os scripts sempre no final da tag body, mas existem necessidades específicas, em que ele é usado no head.
* Script dentro da tag head, é iniciado antes do seu HTML.
* Script no final da tag body, é iniciado depois do HTML.
* Script com arquivo externo - o JavaScript pode ser escrito em um arquivo .js e encaminhado no arquivo .html
```
Ex:

Código em .js (nome de arquivo "teste.js")

alert('Hello World!');


Código em .html

<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="utf-8">
    <title> teste </title>
  </head>
  <body>

    <script src="teste.js"></script>
  </body>
</html>
```

#### Vantagem de usar arquivos externos:
* os códigos ficam separados (HTML em um arquivo JavaScript em outro), isso facilita a manutenção. Se preciso, você consegue alterar algum comando JavaScript sem fazer alteração no HTML
* quando existe um arquivo externo, o navegador se encarrega de fazer cache do mesmo, ou seja, o código não é executado todas as vezes que for carregada a página, ele ficará armazenado no cache e quando for feita alguma alteração, ele renova o cache, acelerando assim o carregamento da página.
