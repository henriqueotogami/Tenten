<div align="center">

# Estudos de banco de dados não relacional (NoSQL) MongoDB.

<img width="auto" src="https://github.com/henriqueotogami/tenten/blob/main/tenten.png?raw=true">

<br>
<br>
<div align="center">
<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/henriqueotogami/tenten">
</div>
<br>
<img src="https://img.shields.io/github/issues/henriqueotogami/tenten">
<img src="https://img.shields.io/github/forks/henriqueotogami/tenten">
<img src="https://img.shields.io/github/stars/henriqueotogami/tenten">
<img src="https://img.shields.io/github/license/henriqueotogami/tenten">
</div>
<br>
<div align=center>
<a href="https://wakatime.com/badge/user/1e53636e-c916-4d50-9ce1-f3ac75a883e3/project/652e9eee-112c-411d-a501-8b225048489c"><img src="https://wakatime.com/badge/user/1e53636e-c916-4d50-9ce1-f3ac75a883e3/project/652e9eee-112c-411d-a501-8b225048489c.svg" alt="wakatime"></a>
<br>
<hr>

Data: 27/01/2023

Curso: [Cod3r | Java 2022 Completo](https://www.udemy.com/course/fundamentos-de-programacao-com-java/)

## Descrição

> Estudos de banco de dados não relacional (NoSQL) MongoDB.

<br>

## Ambiente de Desenvolvimento

### Sistema Operacional: MacOS Monterey - Versão 12.6

### IDE: IntelliJ IDEA Community Edition 2022.2

#### Plugins:

- [Atom Material Icons](https://plugins.jetbrains.com/plugin/10044-atom-material-icons);
- [Codota AI Autocomplete for Java](https://plugins.jetbrains.com/plugin/7638-codota-ai-autocomplete-for-java-and-javascript);
- [GitToolBox](https://plugins.jetbrains.com/plugin/7499-gittoolbox);
- [Nyan Progress Bar](https://plugins.jetbrains.com/plugin/8575-nyan-progress-bar);
- [Rainbow Brackets](https://plugins.jetbrains.com/plugin/10080-rainbow-brackets);
- [Wakatime](https://wakatime.com);
- [Xcode-Dark Theme](https://plugins.jetbrains.com/plugin/13106-xcode-dark-theme);

### Dependências:

- [MongoDB Community Edition - Versão 5.0.14](https://www.mongodb.com/try/download/community)
- [MongoDB Shell - Versão 1.6.2](https://www.mongodb.com/try/download/shell)

#### Instalação do ambiente do MongoDB

##### [How to install Mongodb 5 | latest MAC installation - by Hitesh Choudhary](https://www.youtube.com/watch?v=s1WQ0eEpqqg)

1. Instalar o Homebrew no Mac
```` shell
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
````

2. Instalar Xcode Command Line Tools
````shell
$ xcode-select --install
````

3. Abrindo o Brew Tap
````shell
$ brew tap mongodb/brew
````

4. Instalação da versão 5.0 do MongoDB Community
````shell
$ brew install mongodb-community@5.0
````

5. Inicializar o servidor do MongoDB
````shell
$ brew services start mongodb-community@5.0
````

6. Parar o servidor do MongoDB 
````shell
$ brew services stop mongodb-community@5.0
````

7. Criando o arquivo de configuração do MongoDB
````shell
$ mongod --config /usr/local/etc/mongod.conf --fork
````

8. Criando a pasta de dados do MongoDB
````shell
$ sudo mkdir data
````

9. Criando a pasta do banco de dados do MongoDB
````shell
$ sudo mkdir data/db
````

10. Localizando a pasta BIN dentro da pasta de instalação do MongoDB
````shell
$ /usr/local/Cellar/mongodb-community@5.0/5.0.14/bin
````

11. Adicionar a o diretório da pasta acima no arquivo de endereços do Terminal
````shell
$ sudo nano /etc/paths
````

12. Adicionar a o diretório da pasta acima no arquivo de endereços do Oh My ZSH
````shell
$ sudo nano ~/.zshrc
````

13. Inicializando o banco de dados
````shell
$ mongosh mongod
````

14. Consultando os banco de dados existentes
````shell
$ show dbs
````

## Contribuições

> ### Caso você queira ajudar a melhorar este repositório, qualquer ajuda é bem vinda.

- [x] Faça um **fork** deste repositório (https://github.com/henriqueotogami/tenten/fork);
- [x] Crie um **branch** para adicionar as suas modificações ` git checkout -b meu-novo-recurso `;
- [x] Faça um **commit** ` git commit -am 'feature: Adicionando um novo recurso ...'`;
- [x] Faça um **push** ` git push origin meu-novo-recurso ` ;
- [x] Crie uma nova **pull request** neste repositório.

**Depois que sua solicitação (pull request) for aceita e adicionada (merged) ao ramo principal (branch main), você pode excluir sua branch tranquilamente.**

<div align="center">

<br>

> ### **Muito obrigado, e que a Força esteja com você.**
>
> ### Desenvolvido por **HMAP | Henrique Matheus Alves Pereira** 🦁

</div>
