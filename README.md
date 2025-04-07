# Tutorial de Instalação e Desenvolvimento NODE.JS

### Instalando Node e NPM no PC
```sh
# Instale no seu computador:
sudo apt install nodejs npm
```

### Instalando Node no Projeto
```sh
# Crie uma pasta para o seu projeto e digite:
npm i nodejs
npm i express
```

### Coloque em package.json:
```sh
# Adicione abaixo de "version": "1.0.0",
"type": "module",
```

### Crie um server.js
```sh
import express from 'express';
app.use(express.json());

const app = express();

app.get('/rota', (req, res) => {
    res.send('Rota funcionando!');
});

app.listen(3000);
```

## Tipos de Requests

#### Query Params
- Busca genérica
#### Route Params
- Busca por ID
#### Body Params
{
    "nome":"x","id":y
}
