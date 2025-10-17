# Configurando Alias no git

## Abrir/definir o editor do Git no VS Code

Para definir o VS Code como editor padrão do Git, execute no terminal:

```bash
git config --global core.editor "code"
```

Para verificar o valor atual:

```bash
git config --global --get core.editor
```

## Alias

Você pode adicionar aliases diretamente no arquivo `~/.gitconfig` ou usando o comando `git config`. Exemplo do mesmo alias mostrado no arquivo:

Para criar o alias `s` (curto para `status -s`):

```bash
git config --global alias.s "status -s"
```

Para editar o arquivo `.gitconfig` com o VS Code (se já definiu o editor):

```bash
git config --global --edit
```

Exemplo de `.gitconfig` final:

```ini
[user]
  email = ffbermudes19@gmail.com
  name = Filipe Freitas Bermudes

[core]
  editor = code --wait

[alias]
  s = status -s
  c = add --all && git commit -m
```
