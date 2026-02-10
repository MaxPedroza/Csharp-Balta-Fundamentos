# Instalação do .NET

---

## Objetivo da aula

Nesta aula você vai entender:

- O que precisa instalar para **desenvolver** com .NET.
- A diferença entre **Runtime** e **SDK**.
- Onde baixar com segurança.

---

## O que instalar?

Para começar a programar em .NET você precisa, em geral, de:

1. **.NET SDK** (Software Development Kit)
   - Inclui compilador, templates e a ferramenta de linha de comando `dotnet`.
   - É o pacote usado por **quem desenvolve** aplicações.
2. (Opcional, já incluso no SDK) **.NET Runtime**
   - Usado para **executar** aplicações já prontas.
   - Em servidores e máquinas de usuário final, muitas vezes basta o Runtime.

Para estudar e acompanhar o curso, **instale o SDK**.

---

## Site oficial

Sempre faça o download pelo site oficial:

- https://dotnet.microsoft.com

Lá você encontra:

- Versão **recomendada** (geralmente LTS).
- SDKs para Windows, Linux e macOS.
- Instruções específicas para cada sistema operacional.

---

## Passos gerais de instalação

1. Acesse a página de download do .NET (SDK).
2. Escolha seu sistema operacional (Windows, macOS, Linux).
3. Baixe o instalador recomendado (versão LTS de preferência).
4. Execute o instalador e avance pelo **wizard**.
5. Ao final, abra um terminal/PowerShell e teste com:

```bash
dotnet --version
```

Se aparecer um número de versão (por exemplo, `8.0.100`), a instalação foi concluída com sucesso.

---

## Boas práticas

- Prefira sempre versões **LTS** para projetos de longo prazo.
- Mantenha o SDK relativamente atualizado, mas evite trocar de versão no meio de um projeto sem necessidade.
- Em ambientes de produção, instale apenas o **Runtime** necessário para a aplicação.