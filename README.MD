<br>
<br>
<h1 align="center" >Multilind Orquestrador de Servicos</h1>
<br>
<p align="center"><img width="200"src="assets/img/multilind.jpg"> </p>
<p align="center"> Esse é um repositório que contém o orquestrador dos serviços  do <strong>Multilind</strong>. Ele é respostável por executar todos os contêiners de todos os serviços necessários para a execução do aplicativo.</p>
<br>

# Índice

- [Rode com Docker](#rode-com-docker)
  - [Dependências](#dependências)
  - [Inicialização do Projeto](#inicialização-do-projeto)

## Rode com Docker

### Dependências

Inicialmente, instale localmente as seguintes dependências:

1. Instale o [Docker](https://docs.docker.com/install/linux/docker-ce/ubuntu/);
2. Instale o [Docker Compose](https://docs.docker.com/compose/install/).

### Inicialização do Projeto

1. Na pasta principal do projeto, construa e inicialize a aplicação com o comando:

```bash
make build
```

ou 

```bash
sudo docker-compose up --build
```

2. Todos os serviços serão executados simultaneamente em portas diferentes dentro da aplicação: 
 - Servidor de conteúdo: `http://localhost:8000/api/content`
 - Servidor de controle de usuário: `http://localhost:3000/api/auth`
 - Servidor de criação de arquivos: `http://localhost:5000/api/files`



