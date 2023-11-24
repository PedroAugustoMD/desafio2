### Como rodar

1. Clone o repositório:

```console
https://github.com/PedroAugustoMD/desafio2.git
```

2. Crie um arquivo .env na pasta do seu projeto e edite-o da seguinte forma:

```console
DB_USER=admin
DB_PASS=ZlBrMxsdHPGNjTvE
SECRET=a993db879f6de2e22b9f3a267078ea7e
```

3. Execute os seguintes comandos para iniciar o projeto:

```console
npm install
```

```console
npm run start
```

4. Utilize o insomnia para simular as requisições

- http://localhost:3000/auth/register (POST)
- http://localhost:3000/auth/login (POST)
- http://localhost:3000/user/:id (GET)

### body:

Para criar um usuário.

```json
{
  "name": "",
  "email": "",
  "password": "",
  "telephone": ""
}
```

--

Para Fazer login.

```json
{
  "email": "",
  "password": ""
}
```

Ao autenticar ou criar um cliente você receberá um tolken que será passado no Header para as operações de buscar usuário:
Authorization = Bearer Token
