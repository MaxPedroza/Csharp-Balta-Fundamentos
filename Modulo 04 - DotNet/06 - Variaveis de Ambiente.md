# Variáveis de ambiente

---

## O que são?

**Variáveis de ambiente** são valores armazenados no sistema operacional e que podem ser lidos pelas aplicações.

Elas são úteis para:

- Guardar **configurações** (strings de conexão, chaves de API).
- Diferenciar ambientes (**desenvolvimento**, **homologação**, **produção**).

---

## Exemplos de uso

### Windows (PowerShell)

```powershell
$env:ASPNETCORE_ENVIRONMENT = "Development"
```

### Linux / macOS (bash)

```bash
export ASPNETCORE_ENVIRONMENT=Development
```

Na aplicação .NET, você pode ler esses valores:

```csharp
var ambiente = Environment.GetEnvironmentVariable("ASPNETCORE_ENVIRONMENT");
```

---

## Boas práticas

- **Não** coloque senhas e chaves sensíveis diretamente no código.
- Use variáveis de ambiente (ou gerenciadores de segredo) para esses dados.
- Documente quais variáveis sua aplicação precisa para rodar.

---

## Integração com .NET

Frameworks como o ASP.NET Core possuem suporte integrado para carregar configurações de:

- `appsettings.json`.
- Variáveis de ambiente.
- Linha de comando.

Isso facilita a criação de aplicações configuráveis e seguras.