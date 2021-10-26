# react-atividade-s5-template-JSON-Server

### json-server-s5 API

Arquivo Json para importar no Insomnia: (*Clique direito do mouse -> Salvar link como...*)
- [Download](https://github.com/Kenzie-Academy-Brasil-Developers/react-atividade-s5-json-server-RafaelSchug/blob/main/assets/Insomnia_json-server-s5.json
 "Json para Insomnia")

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

![Criar nova conta](/assets/register.png "Criar nova conta")

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
![Efetuar login](/assets/login.png "Efetuar login")

- - -

### Obter a lista de todos os usuários: (GET)

- /users/

:exclamation:**Auth:** É necessário informar o token de autenticação no header.

![Obter usuários](/assets/get-users.png "Obter usuários")

- - -

### Criar Novo post/mensagem (POST)

- /posts/

:exclamation:**Auth:** É necessário informar o token de autenticação no header.

Para criar um novo post/mensagem, informe no corpo da requisição:


```json
   {
      "message": "Esta é uma mensagem de exemplo.",
      "author": "username",
      "userId": 1
    }
```

![Criar nova mensagem](/assets/newMessage.png "Criar nova mensagem")

- - -

### Obter todos os posts/mensagens cadastradas: (GET)

- /posts/

![Obter todas as mensagens](/assets/get-all-posts.png "Obter todas as mensagens")

- - -

### Obter todos os posts/mensagens cadastradas de um usuário específico: (GET)

- /posts/?author=username

![Obter todas as mensagens especificas](/assets/posts-by-user.png "Obter todas as mensagens especificas")

- - -

### Atualizar um post/mensagem específica: (PATCH)

:exclamation:**Auth:** É necessário informar o token de autenticação no header.

Para atualizar uma mensagem, informe o id da mensagem, com o corpo da requisição no seguinte formato:

- /posts/:id/

```json 
    {
      "message": "Esta é a nova mensagem de exemplo."
    }
```

![Atualizar mensagem específica](/assets/update-post.png "Atualizar mensagem específica")
  