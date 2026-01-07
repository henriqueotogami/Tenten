# Learning MongoDB

> Repositório com exercícios e comandos desenvolvidos durante estudos de banco de dados não relacional (NoSQL) MongoDB.

<div align="center">
<img width="auto" src="https://github.com/henriqueotogami/tenten/blob/main/tenten.png?raw=true">
</div>
<br>
<div align="center">
<img src="https://img.shields.io/github/release-date/henriquemap/tenten">
</div>
<br>
<div align="center">
<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/henriquemap/tenten">
<img src="https://img.shields.io/github/checks-status/henriquemap/tenten/main">
<img src="https://img.shields.io/github/issues/henriquemap/tenten">
</div>
<br>
<div align="center">
<img src="https://img.shields.io/github/forks/henriquemap/tenten?style=flat">
<img src="https://img.shields.io/github/stars/henriquemap/tenten?style=flat">
<img src="https://img.shields.io/github/license/henriquemap/tenten">
</div>
<div align="center">
<br>
<a href="https://wakatime.com/badge/user/1e53636e-c916-4d50-9ce1-f3ac75a883e3/project/652e9eee-112c-411d-a501-8b225048489c"><img src="https://wakatime.com/badge/user/1e53636e-c916-4d50-9ce1-f3ac75a883e3/project/652e9eee-112c-411d-a501-8b225048489c.svg" alt="wakatime"></a>
</div>

## 📋 Sobre o Projeto

Este projeto contém uma coleção de comandos e exemplos práticos desenvolvidos durante o aprendizado de banco de dados não relacional (NoSQL) MongoDB. Os arquivos incluem exercícios práticos que demonstram operações básicas e avançadas do MongoDB, como inserção de dados, consultas, agregações, atualizações e remoções, além de exemplos de relacionamento entre coleções usando `$lookup`.

**Curso:** [Cod3r | Java 2022 Completo](https://www.udemy.com/course/fundamentos-de-programacao-com-java/)

**Data:** 27/01/2023

## 📁 Estrutura do Projeto

### Arquivos de Aula (Lesson Files)

- **lesson-450-basic-commands.txt** - Comandos básicos do MongoDB (criação de banco, coleções, comandos fundamentais)
- **lesson-451-insert-data.txt** - Exemplos de inserção de dados usando `insert()`, `insertOne()` e estruturas aninhadas
- **lesson-453-insert-sao-paulo.txt** - Inserção de dados complexos com arrays aninhados (estados e cidades)
- **lesson-454-queries-database.txt** - Consultas básicas usando `find()`, `findOne()`, filtros e projeções
- **lesson-456-query-with-aggregate.txt** - Agregações básicas usando `$project` e `$group`
- **lesson-457-query-aggregation.txt** - Agregações avançadas com `$match` e `$unwind`
- **lesson-458-update.txt** - Operações de atualização com `update()`, `updateOne()`, `$set` e `$push`
- **lesson-459-remove.txt** - Remoção de documentos com `remove()`, `deleteOne()` e filtros condicionais
- **lesson-460-insert-company.txt** - Inserção de dados com referências entre coleções (empresas e estados)
- **lesson-461-lookup-companies.txt** - Relacionamento entre coleções usando `$lookup` (empresa → estado)
- **lesson-462-lookup-companies.txt** - `$lookup` avançado com arrays aninhados e filtros (`$unwind`, `$addFields`, `$cmp`)

### Estrutura do repositório

```
LICENSE
README.md
images/
  └── mongodb-running.png
lesson-450-basic-commands.txt          # comandos básicos
lesson-451-insert-data.txt             # inserção de dados
lesson-453-insert-sao-paulo.txt        # inserção com arrays aninhados
lesson-454-queries-database.txt        # consultas básicas
lesson-456-query-with-aggregate.txt    # agregações básicas
lesson-457-query-aggregation.txt       # agregações avançadas
lesson-458-update.txt                  # atualização de documentos
lesson-459-remove.txt                  # remoção de documentos
lesson-460-insert-company.txt          # inserção com referências
lesson-461-lookup-companies.txt        # lookup básico
lesson-462-lookup-companies.txt        # lookup avançado
```

## 🛠️ Tecnologias Utilizadas

- **MongoDB** - Banco de dados NoSQL orientado a documentos
- **MongoDB Community Edition** - Versão 5.0.14
- **MongoDB Shell (mongosh)** - Versão 1.6.2
- **Homebrew** - Gerenciador de pacotes para macOS
- **macOS** - Sistema operacional (Monterey 12.6)

## 📝 Funcionalidades Principais

### Comandos Básicos
Os arquivos de lesson demonstram:
- Criação e gerenciamento de bancos de dados
- Criação e manipulação de coleções (tabelas)
- Comandos fundamentais do MongoDB Shell

### Inserção de Dados
- Inserção de documentos simples e complexos
- Uso de `insert()`, `insertOne()` e `insertMany()`
- Estruturas aninhadas com arrays de documentos
- Criação de referências entre coleções usando `ObjectId`

### Consultas e Agregações
- Consultas básicas com `find()` e `findOne()`
- Filtros com operadores (`$or`, `$exists`, `$lt`, etc.)
- Projeções e seleção de campos específicos
- Pipeline de agregação:
  - `$match` - Filtrar documentos
  - `$project` - Selecionar/transformar campos
  - `$group` - Agrupar e calcular agregações
  - `$unwind` - Descompactar arrays
  - `$lookup` - Realizar joins entre coleções
  - `$addFields` - Adicionar campos calculados

### Atualização e Remoção
- Atualização de documentos com `update()`, `updateOne()` e `updateMany()`
- Operadores de atualização: `$set`, `$push`, `$pull`
- Remoção com `remove()`, `deleteOne()` e `deleteMany()`
- Filtros condicionais para operações em lote

### Relacionamentos entre Coleções
- `$lookup` para realizar joins (equivalente a JOIN em SQL)
- Relacionamentos simples (empresa → estado)
- Relacionamentos com arrays aninhados (empresa → cidade dentro de estado)
- Filtros e comparações em relacionamentos complexos

## 🚀 Como Instalar e Configurar

### Pré-requisitos

- macOS (ou sistema compatível com Homebrew)
- Homebrew instalado

### Instalação do MongoDB Community Edition

#### 1. Instalar o Homebrew (se não estiver instalado)
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

#### 2. Instalar Xcode Command Line Tools
```bash
xcode-select --install
```

#### 3. Adicionar o repositório MongoDB ao Homebrew
```bash
brew tap mongodb/brew
```

#### 4. Instalar MongoDB Community Edition 5.0
```bash
brew install mongodb-community@5.0
```

#### 5. Inicializar o servidor MongoDB
```bash
brew services start mongodb-community@5.0
```

#### 6. Parar o servidor MongoDB (quando necessário)
```bash
brew services stop mongodb-community@5.0
```

#### 7. Configurar o MongoDB
```bash
# Criar arquivo de configuração
mongod --config /usr/local/etc/mongod.conf --fork

# Criar diretório de dados
sudo mkdir -p data/db
```

#### 8. Acessar o MongoDB Shell
```bash
mongosh mongod
```

#### 9. Consultar bancos de dados existentes
```bash
show dbs
```

### Referência de Instalação

[How to install Mongodb 5 | latest MAC installation - by Hitesh Choudhary](https://www.youtube.com/watch?v=s1WQ0eEpqqg)

## 📚 Conteúdos Abordados

- ✅ Comandos básicos do MongoDB Shell
- ✅ Criação e gerenciamento de bancos de dados
- ✅ Criação e manipulação de coleções
- ✅ Inserção de documentos (simples e complexos)
- ✅ Consultas básicas com `find()` e `findOne()`
- ✅ Filtros e operadores de consulta
- ✅ Projeções e seleção de campos
- ✅ Pipeline de agregação
- ✅ Operadores de agregação (`$match`, `$project`, `$group`, `$unwind`)
- ✅ Atualização de documentos
- ✅ Operadores de atualização (`$set`, `$push`)
- ✅ Remoção de documentos
- ✅ Relacionamentos entre coleções
- ✅ `$lookup` para realizar joins
- ✅ Trabalho com arrays aninhados
- ✅ Comparações e filtros em relacionamentos complexos

## ⚙️ Como Funciona

### Estrutura de Dados

O projeto trabalha com duas coleções principais:

1. **`estados`** - Armazena informações de estados brasileiros
   - Campos: `nome`, `sigla`, `regiao`, `populacao`
   - Array aninhado: `cidades[]` com informações das cidades

2. **`empresas`** - Armazena informações de empresas
   - Campos: `nome`
   - Referências: `estadoId` ou `cidadeId` (ObjectId)

### Exemplos de Operações

#### Inserção de Dados
```javascript
db.estados.insert({
    nome: "São Paulo",
    sigla: "SP",
    regiao: "Sudeste",
    cidades: [{
        nome: "Campinas",
        area: 795.7,
        populacao: 1081000
    }]
})
```

#### Consultas com Filtros
```javascript
db.estados.find({sigla: "SP"})
db.estados.find({$or: [{sigla: "RJ"}, {sigla: "AC"}]})
```

#### Agregações
```javascript
db.estados.aggregate([
    {$project: {populacao: {$sum: "$cidades.populacao"}, sigla: 1}},
    {$group: {_id: null, populacaoTotal: {$sum: "$populacao"}}}
])
```

#### Lookup (Join entre Coleções)
```javascript
db.empresas.aggregate([
    {$match: {nome: "Bradesco"}},
    {$lookup: {
        from: "estados",
        localField: "estadoId",
        foreignField: "_id",
        as: "estado"
    }}
])
```

## 🔧 Ambiente de Desenvolvimento

### Sistema Operacional
- **macOS Monterey** - Versão 12.6

### Ferramentas
- **MongoDB Community Edition** - Versão 5.0.14
- **MongoDB Shell (mongosh)** - Versão 1.6.2
- **Homebrew** - Gerenciador de pacotes

### IDE Utilizada (Opcional)
- **IntelliJ IDEA Community Edition 2022.2**

#### Plugins Recomendados
- [Atom Material Icons](https://plugins.jetbrains.com/plugin/10044-atom-material-icons)
- [Codota AI Autocomplete for Java](https://plugins.jetbrains.com/plugin/7638-codota-ai-autocomplete-for-java-and-javascript)
- [GitToolBox](https://plugins.jetbrains.com/plugin/7499-gittoolbox)
- [Nyan Progress Bar](https://plugins.jetbrains.com/plugin/8575-nyan-progress-bar)
- [Rainbow Brackets](https://plugins.jetbrains.com/plugin/10080-rainbow-brackets)
- [Wakatime](https://wakatime.com)
- [Xcode-Dark Theme](https://plugins.jetbrains.com/plugin/13106-xcode-dark-theme)

## 📄 Licença

Este projeto está licenciado sob a MIT License - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 📖 Referências

- [MongoDB Documentation](https://www.mongodb.com/docs/)
- [MongoDB Community Edition](https://www.mongodb.com/try/download/community)
- [MongoDB Shell (mongosh)](https://www.mongodb.com/try/download/shell)
- [Curso Cod3r | Java 2022 Completo](https://www.udemy.com/course/fundamentos-de-programacao-com-java/)
- Arquivos de lesson (`lesson-*.txt`) — exemplos práticos de comandos MongoDB

## 🤝 Contribuições

Caso você queira ajudar a melhorar este repositório, qualquer ajuda é bem vinda.

- ✅ Faça um **fork** deste repositório (https://github.com/henriqueotogami/tenten/fork)
- ✅ Crie um **branch** para adicionar as suas modificações `git checkout -b meu-novo-recurso`
- ✅ Faça um **commit** `git commit -am 'feature: Adicionando um novo recurso ...'`
- ✅ Faça um **push** `git push origin meu-novo-recurso`
- ✅ Crie uma nova **pull request** neste repositório

**Depois que sua solicitação (pull request) for aceita e adicionada (merged) ao ramo principal (branch main), você pode excluir sua branch tranquilamente.**
---

### Hashtags
#MongoDB #NoSQL #Database #Learning #Programming #Java #Backend #DatabaseManagement #Aggregation #Lookup #OpenSource #GitHub #CodeExamples #BeginnerProgramming #DatabaseLearning

### Meta Keywords
```
MongoDB, NoSQL, banco de dados, banco de dados não relacional, programação,
comandos MongoDB, agregação, lookup, consultas, inserção de dados, atualização,
remoção, arrays aninhados, relacionamentos, joins, MongoDB Shell, mongosh,
Cod3r, Java, backend, desenvolvimento, código aberto, exemplos práticos,
aprender programação, banco de dados orientado a documentos
```

<br>
<div align="center">
<img width="auto" src="https://github.com/henriqueotogami/tenten/blob/main/resources/kofi-henrique-otogami.jpg?raw=true">
</div>