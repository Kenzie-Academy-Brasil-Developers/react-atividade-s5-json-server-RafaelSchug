# react-atividade-s5-template-JSON-Server

### json-server-s5 API

## ENDEREÇO DE ACESSO:
https://json-server-s5.herokuapp.com

- - -

### Endpoints:

- /register/
- /login/
- /users/
- /posts/

- - -

### Criar nova conta: (POST)

- /register/

Para criar um novo usuário, informe no corpo da requisição:

```json
    {
        "email":"mybestemail@mail.com",
        "password": "123456",
        "name": "username"
    }
```

- - -

### Efetuar Login: (POST)

Para efetuar login, informe o email e senha utilizados no registro:

- /login/

```json
  {
        "email":"mybestemail@mail.com",
        "password": "123456"
  }
```

- - -

### Criar Novo post/mensagem (POST)

- /posts/

**Auth:** É necessário informar o token de autenticação no header.

Para criar um novo post/mensagem, informe no corpo da requisição:


```json
   {
      "message": "Esta é uma mensagem de exemplo.",
      "author": "Nome de usuário",
      "userId": 1
    }
```

- - -

### Obter todos os posts/mensagens cadastradas: (GET)

- /posts/

- - -

### Obter todos os posts/mensagens cadastradas de um usuário específico: (GET)

- /posts/?author=username

- - -

### Atualizar um post/mensagem específica: (PATCH)

**Auth:** É necessário informar o token de autenticação no header.

Para atualizar uma mensagem, informe o id da mensagem, com o corpo da requisição no seguinte formato:

- /posts/:id/

```json 
    {
      "message": "Esta é a nova mensagem de exemplo."
    }
```
  