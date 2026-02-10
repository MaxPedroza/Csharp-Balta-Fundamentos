# VS Code e .NET

---

## Por que usar o VS Code?

O **Visual Studio Code (VS Code)** é um editor leve, multiplataforma e altamente extensível. Ele funciona muito bem com .NET quando combinado com as extensões corretas.

Vantagens:

- Roda em **Windows, Linux e macOS**.
- Suporte a diversas linguagens (C#, JavaScript, HTML, etc.).
- Integração com **Git**, debug, terminal integrado e muito mais.

---

## Extensões recomendadas para C#/.NET

Para ter uma boa experiência com .NET no VS Code, instale:

- **C#** (extensão oficial da Microsoft ou similar)
  - Fornece IntelliSense, highlight de sintaxe, debug etc.
- **.NET Install Tool** (opcional)
  - Ajuda a instalar o runtime/SDK adequado.
- **EditorConfig** (opcional)
  - Ajuda a manter o estilo de código padronizado.

---

## Configurando o ambiente

1. Baixe e instale o VS Code em https://code.visualstudio.com.
2. Instale o **.NET SDK** (se ainda não tiver feito).
3. Abra o VS Code e acesse **Extensions** (`Ctrl+Shift+X`).
4. Procure por **C#** e instale a extensão.
5. Reinicie o VS Code se necessário.

---

## Trabalhando com projetos .NET no VS Code

- Use o **terminal integrado** para rodar comandos `dotnet`:

```bash
dotnet new console -n MeuApp
cd MeuApp
code .
```

- A extensão de C# detecta o projeto e sugere a restauração de dependências.
- Você pode criar configurações de **debug** para executar o projeto apertando `F5`.

---

## Dicas rápidas

- Use o **explorador de arquivos** do VS Code para navegar pelas pastas do projeto.
- Aproveite o **IntelliSense** para descobrir propriedades e métodos.
- Configure atalhos de teclado de acordo com sua preferência para ganhar produtividade.