# Conceitos Nodejs

## 💻Sobre o projeto

Essa será uma aplicação para armazenar repositórios do seu/meu portfólio, que irá permitir a criação, listagem, atualização e remoção dos repositórios, e além disso permitir que os repositórios possam receber "likes".

### **Rotas da aplicação**

Agora que você já está com o template clonado, e pronto para continuar, você deve abrir o arquivo app.js, e completar onde não possui código com o código para atingir os objetivos de cada rota.

- **`POST /repositories`**: A rota deve receber `title`, `url` e `techs` dentro do corpo da requisição, sendo a URL o link para o github desse repositório. Ao cadastrar um novo projeto, ele deve ser armazenado dentro de um objeto no seguinte formato: `{ id: "uuid", title: 'Desafio Node.js', url: 'http://github.com/...', techs: ["Node.js", "..."], likes: 0 }`; Certifique-se que o ID seja um UUID, e de sempre iniciar os likes como 0.
- **`GET /repositories`**: Rota que lista todos os repositórios;
- **`PUT /repositories/:id`**: A rota deve alterar apenas o `title`, a `url` e as `techs` do repositório que possua o `id` igual ao `id` presente nos parâmetros da rota;
- **`DELETE /repositories/:id`**: A rota deve deletar o repositório com o `id` presente nos parâmetros da rota;
- **`POST /repositories/:id/like`**: A rota deve aumentar o número de likes do repositório específico escolhido através do `id` presente nos parâmetros da rota, a cada chamada dessa rota, o número de likes deve ser aumentado em 1;

## ⌨️Instalação

```
git clone https://github.com/OthavioBF/gostack-conceitos-Nodejs.git

```

### **Executando**

Antes de dá start na aplicação você tem que instalar as dependências através do comando:

```tsx
// acessar a pasta do projeto
cd gostack-conceitos-Nodejs

// instala as dependencias
yarn or npm install

// executrando o projeto
yarn dev
```
