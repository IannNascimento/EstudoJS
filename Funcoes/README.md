# Funções
## O que é função
Uma função é um bloco de código projetado para executar uma tarefa específica, essa função só é executada quando "algo" a invoca (chama)

Uma função é definida com a palavra *function*, seguida por um **nome** , seguido por parênteses **( )** 

Os parênteses podem incluir nomes de parâmetros separados por vírgulas:  
**(parametro1, parametro2, ...)**

O código a ser executado, pela função, é colocado dentro de chaves: **{}**

Exemplo:

     <p id="demo"></p>
        
        <script>
        function exFuncao(f1, f2) {
          return f1* f2;
        }
        document.getElementById("demo").innerHTML = exFuncao(4, 3);
        </script>

### Return
A função com return, executa uma determinada tarefa e retorna um valor

    <p id="demo"></p>
    
    <script>
    var x = exFuncao(4, 3);
    document.getElementById("demo").innerHTML = x;
    
    function exFuncao(a, b) {
      return a * b;
    }
    </script>

## Por que utilizar funções?

Você pode reutilizar código: defina o código uma vez e use-o várias vezes.
Você pode reutilizar um código várias vezes com argumentos diferentes para produzir resultados diferentes.
Exemplo 1:

    <p id="demo"></p>
    
    <script>
    function exFuncao(f) {
      return (5/9) * (f-32);
    }
    document.getElementById("demo").innerHTML = exFuncao(77);
    </script>
Resultado = 25

Exemplo 2:

    <p id="demo"></p>
    
    <script>
    function exFuncao(f) {
      return (5/9) * (f-32);
    }
    document.getElementById("demo").innerHTML = exFuncao(32);
    </script>
Resultado = 0

**Acessar uma função sem () retornará a definição da função em vez do resultado da função:**
Exemplo:

    <p id="demo"></p>
    
    <script>
    function exFuncao(f) {
      return (5/9) * (f-32);
    }
    document.getElementById("demo").innerHTML = exFuncao;
    </script>
Resultado = function exFuncao(f) { return (5/9) * (f-32); }
