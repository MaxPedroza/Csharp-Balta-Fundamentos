# Tipos de projeto .NET

---

## Introdução

O .NET permite criar vários tipos de aplicação. A **dotnet CLI** facilita isso com diferentes **templates de projeto**.

---

## Listando templates disponíveis

Para ver todos os tipos de projeto que você pode criar:

```bash
dotnet new --list
```

Isso mostra uma tabela com:

- Nome curto do template (Short Name).
- Linguagem.
- Tipo (console, web, test, etc.).

---

## Exemplos comuns de projetos

### Console

Aplicações de linha de comando:

```bash
dotnet new console -n MeuAppConsole
```

### Web API

APIs REST com ASP.NET Core:

```bash
dotnet new webapi -n MinhaApi
```

### MVC Web App

Aplicações web com páginas, controllers e views:

```bash
dotnet new mvc -n MinhaAppWeb
```

### Biblioteca de classes

Projetos para compartilhar código entre aplicações:

```bash
dotnet new classlib -n MinhaBiblioteca
```

---

## Escolhendo o tipo certo

- **Console** → estudos, ferramentas, automações.
- **Web API / MVC** → serviços e aplicações web.
- **Class Library** → código reutilizável (regras de negócio, utilitários).

Entender os tipos de projeto ajuda a estruturar melhor suas soluções desde o início.