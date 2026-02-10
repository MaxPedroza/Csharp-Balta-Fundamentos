# Estrutura de um app .NET

---

## Arquivos principais em um Console App

Ao criar um projeto console com `dotnet new console`, você verá algo como:

```text
MeuApp/
  MeuApp.csproj
  Program.cs
```

- **`.csproj`**: arquivo de projeto, descreve o tipo de app, dependências, versão de .NET etc.
- **`Program.cs`**: contém o ponto de entrada do programa.

---

## Arquivo .csproj (visão geral)

Exemplo simplificado:

```xml
<Project Sdk="Microsoft.NET.Sdk">
  <PropertyGroup>
    <OutputType>Exe</OutputType>
    <TargetFramework>net8.0</TargetFramework>
  </PropertyGroup>
</Project>
```

- `OutputType` define se é executável (`Exe`) ou biblioteca (`Library`).
- `TargetFramework` indica a versão do .NET alvo.

---

## Estruturas maiores

Em projetos mais complexos, é comum ter:

- Pasta `src/` para código principal.
- Pasta `tests/` para projetos de teste.
- Múltiplos projetos `.csproj` dentro de uma mesma solução.

Exemplo:

```text
MinhaSolucao/
  src/
    MinhaApi/
      MinhaApi.csproj
    MinhaBiblioteca/
      MinhaBiblioteca.csproj
  tests/
    MinhaApi.Tests/
      MinhaApi.Tests.csproj
```

---

## Por que entender a estrutura?

- Facilita navegar em projetos novos.
- Ajuda a organizar melhor seu próprio código.
- Torna mais simples trabalhar em equipe e usar controle de versão (Git).