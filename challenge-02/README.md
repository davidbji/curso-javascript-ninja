// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma(x, y){
    return x + y;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
let soma2 = soma(3,7) + 5;


// Qual o valor atualizado dessa variável?
15

// Declare uma nova variável, sem valor.
let semValor;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function novoValor(){
    let val = 'VALOR'
    semValor = val
    return semValor
}


// Invoque a função criada acima.
novoValor()

// Qual o retorno da função? (Use comentários de bloco).
// Retornou: VALOR

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function teste (x, y, z) {
    if(x * y * z){
        let resultado = x * y * z;
        return resultado
        
    } else {
        console.log("Preencha todos os valores corretamente!")
    }
}


// Invoque a função criada acima, passando só dois números como argumento.
teste(3,2);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
// Retorna: Preencha todos os valores corretamente!
//          undefined

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
teste(3,2,10);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
60;

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/

function teste(x, y, z){
    
    if(x && y == undefined && z == undefined){
        return x;
    } else if (x, y && z == undefined) {
        return x + y;
    }else if(x,y,z){
        let somaDivisao = (x+y)/z;
        return somaDivisao
    } else if(x==undefined,y== undefined, z == undefined){
        return false;
    }else {
        return null;
    }
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
teste(5) // = 5
teste(5,5) // = 10
teste(5,5,2) // = 5
