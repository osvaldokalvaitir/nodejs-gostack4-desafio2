# Node - Desafio 2

[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/osvaldokalvaitir/node-desafio2/blob/master/LICENSE)
![](https://img.shields.io/github/package-json/v/osvaldokalvaitir/node-desafio2.svg)
![](https://img.shields.io/github/last-commit/osvaldokalvaitir/node-desafio2.svg?color=red)
![](https://img.shields.io/github/languages/top/osvaldokalvaitir/node-desafio2.svg?color=yellow)
![](https://img.shields.io/github/languages/count/osvaldokalvaitir/node-desafio2.svg?color=lightgrey)
![](https://img.shields.io/github/languages/code-size/osvaldokalvaitir/node-desafio2.svg)
![](https://img.shields.io/github/repo-size/osvaldokalvaitir/node-desafio2.svg?color=blueviolet)
[![made-for-VSCode](https://img.shields.io/badge/Made%20for-VSCode-1f425f.svg)](https://code.visualstudio.com/)
![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

Aplicação GoBarber usando Node.js, Express, Nunjucks e Sequelize.

## Desafio

Nesse segundo desafio você deve melhorar a aplicação que criamos até agora, o GoBarber.

Até agora criamos a parte do usuário poder agendar um serviço com o prestador, e também vetamos que serviços sejam marcados no mesmo horário, ou em horários que já passaram.

A partir de agora você deve implementar o seguinte:

Crie uma seção para o prestador de serviços acompanhar os agendamentos do dia programados com ele. Essa seção deve incluir as informações do usuário que agendou e também o horário do agendamento.

## Índice

- [Capturas de Tela](#capturas-de-tela)

  - [Login](#login)

  - [Registro](#registro)

  - [Início](#início)

  - [Compromissos](#compromissos)

  - [Agendamentos](#agendamentos)

- [Desenvolvimento](#desenvolvimento)

  - [Configuração do Ambiente](#configuração-do-ambiente)

  - [Instalação do Projeto](#instalação-do-projeto)

  - [Execução do Projeto](#execução-do-projeto)

- [Utilizados no Projeto](#utilizados-no-projeto)

  - [Bibliotecas](#bibliotecas)

  - [APIs](#apis)

  - [Ferramentas](#ferramentas)

## Capturas de Tela

### Login

![SignIn](/.github/assets/signin.png)
Esta é a primeira tela do site, para entrar o usuário terá que digitar seu usuário e senha registrados.
Se o usário não tem ainda um cadastro no site, precisa clicar em `Criar conta grátis` que será redirecionado a página de registro.

### Registro

![SignUp](/.github/assets/signup.png)
Esta tela é responsável pelo registro do usuário onde serão obrigatórios os preenchimentos dos campos como nome, e-mail e senha, escolher uma foto para o avatar e informar se ele é um prestador de serviços.

### Início

![Dashboard](/.github/assets/dashboard.png)
Esta é a tela principal do site, onde você vai encontrar uma lista com todos os prestadores de serviços, poderá iniciar um agendamento com o prestador dê sua preferência, se você for um prestador poderá visualizar seus agendamentos e tem a opção também de sair da sua conta.

### Compromissos

![Appointments](/.github/assets/appointments.png)
Nesta tela, você poderá agendar um horário que esteja disponível do prestador de serviço selecionado.

### Agendamentos

![Schedule](/.github/assets/schedule.png)
Nesta tela estão todos os agendamentos que foram realizados pelos clientes com o prestador de serviço que está logado.

## Desenvolvimento

### Configuração do Ambiente

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/README.md) e siga `Configuração de Ambiente`.

### Instalação do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga `Instalação de Projeto`.

### Execução do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga `Execução de Projeto para Desenvolvimento` ou `Execução de Projeto para Produção`.

## Utilizados no Projeto

### Bibliotecas

- [bcrypt.js](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/bcryptjs.md)

- [Connect Flash](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/connect-flash.md)

- [Connect Loki](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/connect-loki.md)

- [ESLint](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/eslint.md)

- [Express](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express.md)

- [Express Session](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express-session.md)

- [Flatpickr](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/flatpickr.md) - Siga `CDN`

- [Moment](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/moment.md)

- [Multer](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/multer.md)

- [Nodemon](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nodemon.md)

- [Nunjucks](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nunjucks.md)

- [Nunjucks Date Filter Local](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nunjucks-date-filter-local.md)

- [pg](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/pg.md)

- [Sequelize](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/sequelize.md)

- [sequelize-cli](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/sequelize-cli.md)

- [Session File Store](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/session-file-store.md)

### APIs

- **Interna**

  - **Rotas**

    - Prestadores de serviços

      - Lista todos os prestadores de serviços

    - Compromissos

      - Lista todos os compromissos de um prestador
      - Adiciona novos compromissos

    - Disponíveis

      - Lista todos os compromissos de um prestador e de uma data

    - Agendamentos

      - Lista todos os agendamentos de clientes de um prestador

    - Usuários

      - Adiciona novos usuários

    - Sessões

      - Adiciona novas sessões
      - Exclui sessões existentes

    - Arquivos

      - Lista um arquivo

### Ferramentas

- [DBeaver](https://github.com/osvaldokalvaitir/projects-settings/blob/master/database/dbeaver.md)

- [Docker](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/docker.md)

  - Imagem do PostgreSQL: [kartoza-postgis](https://github.com/osvaldokalvaitir/projects-settings/blob/master/virtualization/docker/images/kartoza-postgis.md)
