# Linguagem Compilada e Interpretada

---

## Conceito geral

Toda linguagem precisa ser **traduzida** para algo que o computador entenda. Existem duas abordagens principais:

1. **Compilação**: traduz tudo de uma vez antes da execução.
2. **Interpretação**: lê e executa o código linha a linha, em tempo real.

---

## Linguagens compiladas

Fluxo simplificado:

1. Você escreve o **código-fonte**.
2. O **compilador** analisa, otimiza e gera um **arquivo executável** ou um código intermediário.
3. Você executa o programa pronto.

Vantagens:

- Costumam ser **mais rápidas** em execução.
- Detectam muitos erros **antes** de rodar o programa.

Desvantagens:

- Tempo de compilação pode ser alto em projetos grandes.
- Menos flexíveis para mudar código "ao vivo".

Exemplos: C, C++, Go, muitas vezes C# (compila para IL e depois JIT).

---

## Linguagens interpretadas

Fluxo simplificado:

1. Você escreve o **código-fonte**.
2. Um **interpretador** lê o código e executa **linha a linha**, em tempo de execução.

Vantagens:

- Maior flexibilidade (ideal para scripts, automações rápidas).
- Mais fáceis de testar pequenas mudanças rapidamente.

Desvantagens:

- Geralmente **mais lentas** que linguagens compiladas.
- Alguns erros só aparecem em partes específicas do código, durante a execução.

Exemplos: Python, JavaScript, Ruby, PHP.

---

## Atenção: linguagem vs. implementação

Algumas linguagens podem ter **implementações diferentes**:

- Java é compilado para **bytecode**, que depois é interpretado/otimizado pela JVM.
- C# é compilado para **IL** (Intermediate Language) e depois compilado JIT pelo .NET.

Por isso, muitas vezes se fala em **modelos híbridos**, misturando compilação e interpretação.