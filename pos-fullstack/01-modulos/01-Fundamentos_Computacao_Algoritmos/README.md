# Fundamentos de Computação e Algoritmos em JavaScript

## 📌 Introdução
Este documento apresenta um resumo completo sobre os fundamentos da computação e a implementação de algoritmos utilizando JavaScript. Ele aborda desde conceitos básicos até tópicos mais avançados, fundamentais para o desenvolvimento de software eficiente.

---

## 🖥️ Fundamentos da Computação
### 1️⃣ O que é Computação?
Computação é o estudo de processos que envolvem o armazenamento, processamento e transmissão de informações por meio de dispositivos eletrônicos.

### 2️⃣ Componentes de um Computador
- **Hardware**: CPU, Memória RAM, SSD/HDD, Periféricos.
- **Software**: Sistemas operacionais, aplicativos e programas.

### 3️⃣ Representação da Informação
- **Sistema Binário**: Base 2 (0 e 1).
- **Tipos de Dados**: Inteiros, ponto flutuante, caracteres, booleanos.
- **Conversão de Bases**: Binário, Decimal, Hexadecimal.

### 4️⃣ Estruturas de Dados
- Arrays
- Objetos
- Pilhas (Stacks)
- Filas (Queues)
- Listas Ligadas (Linked Lists)
- Árvores (Trees)
- Grafos (Graphs)

---

## 📌 Fundamentos de Algoritmos
### 1️⃣ O que é um Algoritmo?
Um algoritmo é uma sequência de passos bem definidos para resolver um problema.

### 2️⃣ Características dos Algoritmos
- Finito
- Definido
- Bem estruturado

### 3️⃣ Estruturas de Controle
- **Sequência**: Execução linear de instruções.
- **Decisão (Condicionais)**: `if`, `else`, `switch`.
- **Repetição (Loops)**: `for`, `while`, `do while`.

### 4️⃣ Complexidade de Algoritmos
- **Notação Big-O**: O(1), O(n), O(log n), O(n²), etc.
- Eficiência de tempo e espaço.

### 5️⃣ Tipos de Algoritmos
- **Dividir para Conquistar** (Merge Sort, Quick Sort).
- **Guloso** (Dijkstra, Kruskal).
- **Programação Dinâmica** (Fibonacci, Problema da Mochila).

---

## 🚀 Algoritmos em JavaScript

### 1️⃣ Variáveis e Tipos de Dados
```js
let nome = "João";
const idade = 25;
let ativo = true;
```

### 2️⃣ Estruturas Condicionais
```js
if (idade >= 18) {
    console.log("Maior de idade");
} else {
    console.log("Menor de idade");
}
```

### 3️⃣ Estruturas de Repetição
```js
for (let i = 0; i < 5; i++) {
    console.log("Número: " + i);
}
```

### 4️⃣ Funções
```js
function somar(a, b) {
    return a + b;
}
console.log(somar(5, 3));
```

### 5️⃣ Estruturas de Dados
#### Arrays
```js
let numeros = [1, 2, 3, 4, 5];
numeros.push(6);
console.log(numeros);
```

#### Objetos
```js
let pessoa = {
    nome: "Carlos",
    idade: 30,
    profissao: "Desenvolvedor"
};
console.log(pessoa.nome);
```

### 6️⃣ Algoritmos Comuns
#### Bubble Sort
```js
function bubbleSort(arr) {
    let len = arr.length;
    for (let i = 0; i < len; i++) {
        for (let j = 0; j < len - i - 1; j++) {
            if (arr[j] > arr[j + 1]) {
                [arr[j], arr[j + 1]] = [arr[j + 1], arr[j]];
            }
        }
    }
    return arr;
}
console.log(bubbleSort([5, 2, 9, 1, 5, 6]));
```

#### Busca Binária
```js
function buscaBinaria(arr, alvo) {
    let inicio = 0, fim = arr.length - 1;
    while (inicio <= fim) {
        let meio = Math.floor((inicio + fim) / 2);
        if (arr[meio] === alvo) return meio;
        else if (arr[meio] < alvo) inicio = meio + 1;
        else fim = meio - 1;
    }
    return -1;
}
console.log(buscaBinaria([1, 2, 3, 4, 5, 6], 4));
```

---

## 📚 Conclusão
Este documento apresentou os principais conceitos de computação e algoritmos utilizando JavaScript. Com esse conhecimento, é possível criar soluções eficientes para problemas computacionais diversos.

Se deseja aprofundar-se, recomenda-se estudar estruturas de dados avançadas, algoritmos de ordenação e técnicas de otimização.

### 🔗 Recursos Extras
- [MDN JavaScript Guide](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
- [Big-O Cheat Sheet](https://www.bigocheatsheet.com/)
- [Estruturas de Dados e Algoritmos com JavaScript](https://eloquentjavascript.net/)

Happy coding! 🚀
