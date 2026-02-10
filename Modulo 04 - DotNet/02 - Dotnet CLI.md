# dotnet CLI

---

## O que é a dotnet CLI?

A **dotnet CLI** é a ferramenta de linha de comando do .NET. Com ela, você consegue:

- Criar novos projetos.
- Restaurar pacotes.
- Compilar e executar aplicações.
- Gerenciar múltiplas versões do SDK.

Tudo isso diretamente pelo terminal (PowerShell, CMD, bash, etc.).

---

## Verificando a versão instalada

Para conferir se o .NET está instalado e qual versão você tem:

```bash
dotnet --version
```

Esse comando retorna algo como `8.0.100`, indicando a versão atual do SDK em uso.

---

## Listando versões instaladas

Você pode ter **várias versões** do .NET na mesma máquina. Para listar todas as versões instaladas:

```bash
dotnet --list-sdks

dotnet --list-runtimes
```

- `--list-sdks`: mostra todos os SDKs instalados.
- `--list-runtimes`: mostra todos os runtimes instalados.

---

## Alterando versões usadas

O .NET escolhe o SDK com base em:

1. O que está instalado na máquina.
2. Arquivos de configuração do projeto (`global.json`, por exemplo).

Quando um arquivo `global.json` está presente em uma pasta, ele pode forçar o uso de uma versão específica de SDK para aquela solução, garantindo consistência entre todos os desenvolvedores.

Exemplo (apenas ilustrativo de conteúdo):

```json
{
  "sdk": {
    "version": "8.0.100"
  }
}
```

---

## Aceitando certificados (casos específicos)

Em alguns sistemas operacionais (como macOS ou ambientes corporativos), ao rodar `dotnet` pela primeira vez, você pode receber avisos sobre **certificados HTTPS**.

Normalmente, basta seguir as instruções exibidas no terminal ou na documentação para confiar nos certificados usados pelo ASP.NET durante o desenvolvimento.

---

## Por que aprender a CLI?

Mesmo usando uma IDE gráfica, saber usar a CLI traz vantagens:

- Funciona em qualquer sistema operacional.
- Útil em servidores, pipelines de CI/CD e automações.
- Dá mais controle e entendimento sobre o que a IDE faz "por trás".