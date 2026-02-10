# Compilada e Interpretada na Prática

---

## Comparando os modelos

| Característica      | Compilada                        | Interpretada                     |
|---------------------|----------------------------------|----------------------------------|
| Momento da tradução | Antes da execução                | Durante a execução               |
| Desempenho          | Geralmente maior                 | Geralmente menor                 |
| Detecção de erros   | Em tempo de compilação           | Em tempo de execução             |
| Distribuição        | Executável pronto ou bytecode    | Código-fonte + interpretador     |

---

## Exemplo de compilação (C#)

```bash
csc Programa.cs   # Compila o arquivo Programa.cs
Programa.exe      # Executa o binário gerado
```

Nesse fluxo:

- O código é analisado pelo **compilador C#**.
- Se houver erros de sintaxe ou tipos, a compilação falha.
- Se der tudo certo, é gerado um executável (ou assembly .NET).

---

## Exemplo de interpretação (Python)

```bash
python script.py
```

Nesse fluxo:

- O interpretador Python lê o arquivo `script.py`.
- Cada linha é analisada e executada na hora.

Se existir um erro em uma função que **não é chamada**, o programa pode rodar sem reclamar — até o ponto em que aquela parte do código é executada.

---

## Modelos híbridos

Muitas plataformas modernas misturam os dois mundos:

- **Java**: código `.java` → compilado para **bytecode** `.class` → executado/otimizado pela JVM.
- **C# / .NET**: código `.cs` → compilado para **IL** → compilado JIT (Just-In-Time) em tempo de execução.

Esse modelo tenta equilibrar:

- **Performance** de linguagens compiladas.
- **Flexibilidade** de linguagens interpretadas.

Entender essa diferença é essencial para saber o que está acontecendo "por baixo dos panos" quando você aperta **F5** na sua IDE.