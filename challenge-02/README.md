# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function Soma(x, y) {
    return x+y;
};

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var somar = Soma(1, 2);
somar += 5;

// Qual o valor atualizado dessa variável?
soma == 8;

// Declare uma nova variável, sem valor.
var novaVariavel;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function Atribuicao(variavel) {
    variavel = 5;
    return `O valor da novaVariavel agora é 5.`
}

// Invoque a função criada acima.
novaVariavel = Atribuicao(novaVariavel);

// Qual o retorno da função? (Use comentários de bloco).
'O valor da novaVariavel agora é 5.'

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function Matematica (x, y, z) {
    if((x == null) || (y == null) || (z == null)) {
        return 'Preencha todos os valores corretamente!';
    }else {
        return (x*y*z) + 2;
    }
}

// Invoque a função criada acima, passando só dois números como argumento.
Matematica (1, 2); // 'Preencha todos os valores corretamente!'

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).


// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
Matematica (1, 2, 3); //8

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).


/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function Matematica (x, y, z) {
    if((x != null) && (y == null) && (z == null )) { //se só 1 argumento, retorna o proprio argumento
        return x;
    }else if((x != null) && (y != null) && (z == null)) { //se 2 argumentos, retorna a soma dos dosi argumentos
        return x+y;
    }else if((x != null) && (y != null) && (z != null)) { //se 3 argumentos, retorna a soma do 1º com o 2º dividido pelo 3º
        return (x+y) / z
    }else if((x == null) && (y == null) && (z == null)) { //se nenhum argumento, retorna valor booleano false
        return false;
    }else { //se nenhum dos de cima, retorna vazio (null)
        return null
    }
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.

```