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

![Criar nova conta](https://raw.githubusercontent.com/Kenzie-Academy-Brasil-Developers/react-atividade-s5-json-server-RafaelSchug/main/assets/register.png?token=ALGDUMW6WGAQUW2MC4B5JTTBQCDXQ "Criar nova conta")

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
![Efetuar login](https://raw.githubusercontent.com/Kenzie-Academy-Brasil-Developers/react-atividade-s5-json-server-RafaelSchug/main/assets/login.png?token=ALGDUMW2FA2ZQUB5OEI6P6DBQCEPQ "Efetuar login")

- - -

### Criar Novo post/mensagem (POST)

- /posts/

**Auth:** É necessário informar o token de autenticação no header.

Para criar um novo post/mensagem, informe no corpo da requisição:


```json
   {
      "message": "Esta é uma mensagem de exemplo.",
      "author": "username",
      "userId": 1
    }
```

![Criar nova mensagem](https://raw.githubusercontent.com/Kenzie-Academy-Brasil-Developers/react-atividade-s5-json-server-RafaelSchug/main/assets/newMessage.png?token=ALGDUMX4SAY5F66MBXTWOJ3BQCD54 "Criar nova mensagem")

- - -

### Obter todos os posts/mensagens cadastradas: (GET)

- /posts/

![Obter todas as mensagens](https://raw.githubusercontent.com/Kenzie-Academy-Brasil-Developers/react-atividade-s5-json-server-RafaelSchug/main/assets/get-all-posts.png?token=ALGDUMSUWZE7FQ4D2CL6EZTBQCEKQ "Obter todas as mensagens")

- - -

### Obter todos os posts/mensagens cadastradas de um usuário específico: (GET)

- /posts/?author=username

![Obter todas as mensagens especificas](https://raw.githubusercontent.com/Kenzie-Academy-Brasil-Developers/react-atividade-s5-json-server-RafaelSchug/main/assets/posts-by-user.png?token=ALGDUMTJAAL7KPUS4CNQUY3BQCENI "Obter todas as mensagens especificas")

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

![Atualizar mensagem específica](https://raw.githubusercontent.com/Kenzie-Academy-Brasil-Developers/react-atividade-s5-json-server-RafaelSchug/main/assets/update-post.png?token=ALGDUMQESCPGMVT2CDLXA4TBQCEF2 "Atualizar mensagem específica")
  