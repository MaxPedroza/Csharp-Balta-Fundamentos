# Debug em aplicações .NET

---

## O que é debug?

**Debug** é o processo de executar o programa passo a passo para:

- Entender o fluxo de execução.
- Inspecionar valores de variáveis.
- Descobrir a causa de erros e comportamentos inesperados.

---

## Ferramentas

- Em IDEs como **VS Code** ou **Visual Studio**, você tem:
  - Breakpoints (pontos de parada).
  - Inspeção de variáveis.
  - Pilha de chamadas (call stack).
  - Execução passo a passo (Step Over, Step Into, Step Out).

---

## Exemplo de uso no VS Code

1. Abra o projeto no VS Code.
2. No arquivo `Program.cs`, clique à esquerda da linha para adicionar um **breakpoint**.
3. Pressione `F5` para iniciar o debug.
4. Quando a execução parar no breakpoint, observe:
   - Valores das variáveis.
   - Janelas de **Locals**, **Watch** e **Call Stack**.

---

## Logs e mensagens

Além do debug interativo, você pode usar:

- `Console.WriteLine` em aplicações console.
- Frameworks de logging (Serilog, NLog, ILogger do ASP.NET Core, etc.).

Boas mensagens de log facilitam a descoberta de problemas em ambientes onde o debug interativo não é possível (por exemplo, em produção).

---

## Boas práticas de debug

- Reproduza o problema em um ambiente de teste sempre que possível.
- Faça pequenas alterações e teste frequentemente.
- Use breakpoints condicionais quando o erro só ocorre em situações específicas.

Com prática, o debug se torna uma das ferramentas mais poderosas do seu dia a dia como desenvolvedor.