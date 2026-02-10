# Runtime e SDK

---

## Diferença entre Runtime e SDK

Para trabalhar com .NET, você encontra dois tipos principais de instalação:

- **Runtime**
  - Responsável por **executar** as aplicações.
  - Contém o mínimo necessário para rodar programas já compilados.
- **SDK (Software Development Kit)**
  - Conjunto de ferramentas para **desenvolver** aplicações.
  - Inclui compilador, templates de projeto, ferramentas de linha de comando (CLI) etc.

---

## Quando usar cada um?

- **Somente Runtime**
  - Máquinas de produção (servidores).
  - Máquinas de clientes que apenas **executam** a aplicação.
- **SDK**
  - Ambiente de desenvolvimento (seu computador, CI, etc.).
  - Necessário para criar, compilar e testar aplicações.

O SDK já inclui o runtime necessário para o desenvolvimento.

---

## Tipos de runtimes

No .NET moderno, os runtimes podem ser separados em:

- **.NET Runtime** (básico, para aplicações de console/gerais).
- **ASP.NET Core Runtime** (para aplicações web).
- **Desktop Runtime** (para aplicações desktop específicas, em cenários suportados).

Essa divisão permite pacotes menores, específicos para o tipo de aplicação.

---

## Onde baixar?

Sempre utilize o site oficial:

- [https://dotnet.microsoft.com](https://dotnet.microsoft.com)

Você pode ir direto à página de uma versão com URLs no formato:

```text
https://dotnet.microsoft.com/download/dotnet-core/3.1
```

(Exemplo com a versão 3.1 citada no material original.)

---

## CLI – `dotnet`

Depois de instalar o SDK, você terá acesso à **dotnet CLI**:

- Verificar versão instalada.
- Listar versões.
- Criar novos projetos.
- Restaurar pacotes, compilar e executar.

Ela será usada com frequência nos próximos módulos.