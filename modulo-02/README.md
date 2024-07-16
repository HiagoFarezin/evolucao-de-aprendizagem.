![](https://i.imgur.com/xG74tOh.png)

# EXEMPLO - Conteúdo modelo no GitHub

## Conteúdos a serem trabalhados nesse módulo:

Funções
Tipos de dados
Tipos Utilitários
Métodos de Arrays

## O que eu já sei sobre os assuntos que serão abordados nesse módulo?

Função:
Aprendemos que as funções em TypeScript são semelhantes às funções em JavaScript, mas com a adição de tipos para parâmetros e retorno; 

outro exemplo:

function add(a: number, b: number): number {
    return a + b;
}

const result = add(5, 3); // 8


Funções Anônimas e Arrow Functions
TypeScript também suporta funções anônimas e arrow functions; ex:

const multiply = (a: number, b: number): number => {
    return a * b;
}

const result = multiply(4, 5); // 20


Tipos de Dados
Aprendemos que o TypeScript adiciona tipagem estática a JavaScript, o que significa que você pode definir o tipo de variáveis, parâmetros e retornos de funções; ex:

number: Números
string: Cadeias de caracteres
boolean: Valores booleanos (true ou false)
array: Arrays, que podem ser tipados com elementos do mesmo tipo
tuple: Arrays com um número fixo de elementos de tipos específicos
enum: Enumerações
any: Um tipo que pode ser qualquer coisa
void: Indica que uma função não retorna um valor
null e undefined: Representam valores nulos e indefinidos

outro exemplo:

let num: number = 10;
let name: string = "TypeScript";
let isValid: boolean = true;
let numbers: number[] = [1, 2, 3];
let tuple: [number, string] = [1, "one"];

enum Color {
    Red,
    Green,
    Blue
}
let color: Color = Color.Green;

Tipos Utilitários
Aprendemos que o TypeScript fornece vários tipos utilitários para facilitar manipulações comuns de tipos. Alguns dos mais utilizados são:

Partial<T>: Torna todas as propriedades de T opcionais.
Required<T>: Torna todas as propriedades de T obrigatórias.
Readonly<T>: Torna todas as propriedades de T somente leitura.
Pick<T, K>: Cria um tipo composto apenas por um conjunto de propriedades de T.
Omit<T, K>: Cria um tipo a partir de T, excluindo um conjunto de propriedades.

outro exemplo:

interface User {
    id: number;
    name: string;
    email?: string;
}

const partialUser: Partial<User> = { name: "Alice" };
const requiredUser: Required<User> = { id: 1, name: "Bob", email: "bob@example.com" };
const readonlyUser: Readonly<User> = { id: 2, name: "Charlie", email: "charlie@example.com" };
const pickedUser: Pick<User, "id" | "name"> = { id: 3, name: "David" };
const omittedUser: Omit<User, "email"> = { id: 4, name: "Eve" };

Métodos de Arrays
Aprendemos que  "arrays em TypeScript" herdam os métodos do JavaScript, permitindo manipulações poderosas. Aqui estão alguns métodos comuns:

push: Adiciona elementos ao final do array.
pop: Remove o último elemento do array.
shift: Remove o primeiro elemento do array.
unshift: Adiciona elementos no início do array.
map: Cria um novo array com os resultados de chamar uma função para cada elemento.
filter: Cria um novo array com todos os elementos que passam no teste de uma função.
reduce: Aplica uma função a um acumulador e a cada elemento do array (da esquerda para a direita) para reduzi-lo a um único valor.

outro exemplo:

let numbers = [1, 2, 3, 4, 5];

numbers.push(6); // [1, 2, 3, 4, 5, 6]
numbers.pop(); // [1, 2, 3, 4, 5]

numbers.shift(); // [2, 3, 4, 5]
numbers.unshift(1); // [1, 2, 3, 4, 5]

const squares = numbers.map(num => num * num); // [1, 4, 9, 16, 25]
const evens = numbers.filter(num => num % 2 === 0); // [2, 4]

const sum = numbers.reduce((total, num) => total + num, 0); // 15






## O que quero aprender sobre os assuntos que serão abordados nesse módulo?




Funções em TypeScript

Objetivo: Compreender como criar e utilizar funções em TypeScript, incluindo funções nomeadas, anônimas e arrow functions.
Detalhes:
Sintaxe de funções nomeadas e anônimas.
Uso de tipos para parâmetros e retorno de funções.
Diferenças entre funções tradicionais e arrow functions.

Tipos de Dados em TypeScript

Objetivo: Entender os diferentes tipos de dados em TypeScript e como usá-los para garantir a segurança de tipos no código.
Detalhes:
Tipos primitivos (number, string, boolean).
Arrays e tuplas.
Enums.
Tipos especiais (any, void, null, undefined).
Interfaces e tipos personalizados.

Tipos Utilitários em TypeScript

Objetivo: Aprender a usar tipos utilitários para manipular e transformar tipos existentes de maneira eficiente.
Detalhes:
Uso de Partial, Required, Readonly, Pick, Omit e outros utilitários.
Aplicações práticas desses tipos em diferentes cenários.

Métodos de Arrays

Objetivo: Dominar os métodos de arrays disponíveis em TypeScript para manipular coleções de dados de maneira eficaz.
Detalhes:
Métodos de mutação (push, pop, shift, unshift).
Métodos de iteração e transformação (map, filter, reduce).
Exemplos práticos de uso desses métodos em diferentes contextos.
Específicos que você pode querer aprender:
Funções em TypeScript:

Como definir e chamar funções.
Como utilizar tipos para parâmetros e retornos.
Diferenças e vantagens das arrow functions.
Tipos de Dados em TypeScript:

Como declarar e usar diferentes tipos de dados.
Vantagens de usar tipos seguros.
Como definir tipos personalizados usando interfaces e type aliases.
Tipos Utilitários em TypeScript:

Como tornar propriedades opcionais ou obrigatórias.
Como criar tipos somente leitura.
Como selecionar ou omitir propriedades de um tipo.
Métodos de Arrays:

Como adicionar e remover elementos em arrays.
Como transformar e filtrar arrays de maneira eficiente.
Como usar reduce para agregação de dados.


## Minha evolução: o que aprendi sobre os assuntos que foram abordados nesse módulo?
"construção"
