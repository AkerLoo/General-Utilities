#### Documentação **📄**

[Mdn web docs ](https://developer.mozilla.org/pt-BR/)👏

[Sintaxe Básica Markdown](https://www.markdownguide.org/basic-syntax/) 👏

[Git hub Docs](https://docs.github.com/pt) 👏

[Documentação WSL](https://docs.microsoft.com/pt-br/windows/wsl/install#check-which-version-of-wsl-you-are-running) 👏


------------------------------------------------------------------------------------------------------------------------------


### Para criar uma chave SSH publica, siga os seguintes passos:

 **Obs:** Vão ser geradas duas chaves uma .pub (publica) e outra privada.

**Passo 1** - Abra o Git Bash

**Passo 2** - Inserir o seguinte comando:

```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

**Passo 3** - Aperte enter e depois coloque sua senha.

**Passo 4** - Ir verificar o caminho onde foi instalado a chave usando [`Cd /.../.../.../`] e depois listar usando  [`ls`]

**Passo 5** - Para ver o conteúdo dentro do arquivo criado (SSH criptografado) execute o seguinte comando:

```
cat id_ed25519.pub
```

**Passo 6** - Copiar a o conteúdo da pasta e colar no local de chaves SSH no Git Hub para cadastra a chave em si.

**Passo 7** - Executar o Agente SSH com o comando:

```
eval $(ssh-agent -s) 
```

**Passo 8** - Executar o seguinte comando para passar a chave privada para o Agente SSH:

```
ssh-add ~/.ssh/id_ed25519
```

