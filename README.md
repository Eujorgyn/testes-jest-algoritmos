# Algoritmos fundamentais com testes unitários (Jest)

Seis algoritmos clássicos em **JavaScript (Node.js)**, escritos com **programação defensiva** e **clean code**. Todos têm **testes unitários em Jest**: são 25 testes, todos passando.

![Node.js](https://img.shields.io/badge/Node.js-18%2B-339933?logo=node.js&logoColor=white)
![Jest](https://img.shields.io/badge/testes-Jest-C21325?logo=jest&logoColor=white)

| Algoritmo | Arquivo | Função |
|---|---|---|
| Número primo | `funcoes/numeroprimo.js` | `verificarPrimo(numero)` |
| Somatório | `funcoes/somatorio.js` | `calcularSomatorio(numeros)` |
| Fibonacci | `funcoes/fibonacci.js` | `gerarFibonacci(quantidadeTermos)` |
| MDC (Euclides) | `funcoes/mdc.js` | `calcularMDC(a, b)` |
| Quicksort | `funcoes/quicksort.js` | `quicksort(numeros)` |
| Contagem | `funcoes/contagem.js` | `contarValores(dados, limite)` |

## Como executar

O projeto fica na pasta `Entregavel-1-testes`. Pra rodar:

```bash
cd Entregavel-1-testes
npm install
npm test          # roda os 25 testes
npm start         # programa interativo no terminal
```

Saída esperada dos testes:

```
Test Suites: 6 passed, 6 total
Tests:       25 passed, 25 total
```

## Boas práticas aplicadas

- **Validação de entrada:** antes de calcular, cada função confere o tipo e o intervalo dos valores (`validacoes.js`).
- **Erros claros:** tipo errado gera `TypeError` e valor fora do permitido gera `RangeError` (por exemplo, Fibonacci negativo ou MDC de 0 e 0).
- **Responsabilidade única:** cada algoritmo fica em um arquivo, separado da entrada e saída.
- **Sem efeitos colaterais:** o `quicksort` devolve um novo array e não altera o original.
- **Otimizações:** o teste de primo só verifica divisores até a raiz quadrada, e o MDC aceita negativos.

## Estrutura

```
Entregavel-1-testes/
├── funcoes/          # algoritmos (um por arquivo) + validações
├── tests/            # testes unitários Jest
├── entregavel_1/     # programa interativo (terminal)
├── entregavel_1_2/   # versão em Java
└── package.json
```

## Autor

**Jorge Gabriel**, estudante de Análise e Desenvolvimento de Sistemas na UNIFOR.
[GitHub](https://github.com/Eujorgyn) · jorgegabrielpinheirofrutuoso@gmail.com
