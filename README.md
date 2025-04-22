Esta é uma API em construção, que será uma API desenvolvida para upload de imagens no servidor, utilizando Node.js, Express, mongoose e multer. A API permite pegar uma imagem, subir para o servidor salvar e exluir do servidor no MongoDB.



## Funcionalidades:

* GET:/pictures: Retorna a lista de completa de imagens.
* POST: adiciona uma imagem.
* DELETE: remove uma imagem indesejada.


## Estrutura do projeto

- **multer.js**:
- **PictureController.js**:
- **Picture.js**:Modelo Mongoose para imagens.
- **picture.js**:Rotas para gerenciar imagens.
- **app.js**:Configuração do servidor Express e rotas.
- **db.js**:Conexão com o banco de dados MongoDB.
- **index.html**:Interface web para o usuário.
- **script.js**:Lógica do frontend para interagir com a API.
- **styles.css**:Estilos para a interface.

## Tecnologia Usadas:
- **Node.js**:Ambiente de execução para JavaScript no backend
- **Mongoose**:Biblioteca para modelagem de objetos e interação com o MongoDB.
- **dotenv**:Biblioteca para carregar variáveis de ambiente a partir de um arquivo
- **MongoDB Atlas**:Banco de dados NoSQL hospedado na nuvem.

1. GET /pictures  
Retorna a lista completa de imagens disponíveis.

Exemplo de resposta:
```json
[
    {
        "_id": "664e8b472a4c2f1e8c3c56b9",
        "filename": "foto1.jpg",
        "path": "uploads/foto1.jpg",
        "createdAt": "2025-04-20T10:23:45.678Z"
    },
    {
        "_id": "664e8c152a4c2f1e8c3c56ba",
        "filename": "foto2.png",
        "path": "uploads/foto2.png",
        "createdAt": "2025-04-20T10:25:10.345Z"
    }
]
```
 ## Pré-requisitos
- **Node.js instalado.**
- **MongoDB configurado.**
- **Variáveis de ambiente configuradas no arquivo `.env`:**

## Instalação
1. Clone o repositório:

```bash
   git clone <url-do-repositorio>
   cd upload-img
```
2. Instale as dependências:
```bash
  npm install
```

5.Acesse a aplicação em http://localhost:4000.

3.Configure o arquivo .env com suas credenciais do MongoDB.

4. Inicie o servidor:
```bash
  npm start
```
A API estará disponível em [http://localhost:4000](http://localhost:4000). 
