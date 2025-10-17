# Configurando dependências do projeto

[Voltar](./README.md)

## Conventional commits

O padrão dos commits será seguindo o modelo convencional commits
[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

## Instalação de dependências

- Iniciar o projeto node

  -Y garante que seja criado o packet.json com valores padrão

```bash
npm init -y
```

- Dependência para garantir padrão de commits

```bash
npm i -D git-commit-msg-linter
```

- Dependência para o funcionamento do typescript

```bash
npm i -D typescript @types/node
```

- Arquivo tsconfig.json

```json
{
  "compilerOptions": {
    "outDir": "./dist",
    "module": "commonjs",
    "target": "es2019",
    "esModuleInterop": true,
    "allowJs": true
  }
}
```
