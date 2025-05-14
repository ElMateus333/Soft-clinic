# Sistema de Gestão de Clínicas
Sistema de Gestão de Clínicas - API RESTful para gerenciar múltiplas clínicas, incluindo autenticação, autorização, pacientes, médicos, funcionários, medicamentos, clínicas, consultas, prescrições, faturas e pagamentos. Gerencie todos os dados da clínica com facilidade.

## Introdução
Esta é uma API REST que implementa um sistema de gestão de clínicas médicas. Ela fornece endpoints para diferentes entidades no sistema (pacientes, médicos, funcionários, etc.), cada uma com suas próprias operações CRUD. Ela também oferece diferentes papéis e níveis de autorização para diferentes usuários. A API usa MongoDB para persistência e é construída usando Node.js e o framework Express.

## Tecnologias
As seguintes tecnologias foram usadas para desenvolver a plataforma:

- Node.js
- Express
- MongoDB
- Mongoose
- Morgan
- bcrypt
- easyinvoice
- express-validator
- fs
- jsonwebtoken
- mongoose-sequence
- mongoose-validator
- multer
- nodemailer
- stripe
- validatorjs

## Recursos

- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)

## Requisitos

* Node.js
* npm
* MongoDB

## Ferramentas

- [Visual Studio Code](https://code.visualstudio.com/)
- [MongoDB Compass](https://www.mongodb.com/products/compass)
- [Robo 3T](https://robomongo.org/)
- [Postman](https://www.postman.com/)

## Configuração

A API usa as seguintes variáveis de ambiente:

* `PORT` - a porta na qual a API vai escutar por requisições.
* `MONGODB_URI` - a URL do banco de dados MongoDB para conectar.
* `MONGODB_LOCAL` - a URL do banco de dados MongoDB local para conectar.
* `SECRET_KEY` - uma string usada para o bcrypt para proteger a aplicação e criptografar senhas de usuários.
* `SECRET_KEY_STRIPE` - uma string usada para autenticar com a API de processamento de pagamentos Stripe e tratar transações de forma segura.

## Instalação
Para instalar a plataforma e suas dependências, siga os seguintes passos:

## Funcionalidades

O projeto possui diversas funcionalidades, incluindo:

- Cadastrar pacientes: Permite que pacientes se cadastrem no centro médico.
- Autenticar usuários: Permite que usuários se autentiquem no centro médico.
- Gerenciar consultas: Permite que usuários gerenciem consultas, incluindo adicionar consultas, obter todas as consultas e mais.
- Gerenciar prescrições: Permite que usuários gerenciem prescrições, incluindo adicionar prescrições e obter todas as prescrições.
- Gerenciar faturas: Permite que usuários gerenciem faturas, incluindo adicionar faturas e obter todas as faturas.
- Gerenciar pagamentos: Permite que usuários gerenciem pagamentos, incluindo adicionar pagamentos e obter todos os pagamentos.


## Endpoints

A API implementa os seguintes endpoints:

* `/register` - Requisição POST para cadastrar um novo paciente.
* `/auth` - Requisição POST para autenticar um usuário.
* `/doctor` - Operações CRUD em médicos.
* `/patient` - Operações CRUD em pacientes.
* `/employee` - Operações CRUD em funcionários.
* `/medicine` - Operações CRUD em medicamentos.
* `/clinic` - Operações CRUD em clínicas.
* `/appointment` - Operações CRUD em consultas.
* `/prescription` - Operações CRUD em prescrições.
* `/invoice` - Operações CRUD em faturas.
* `/payment` - Operações CRUD em pagamentos.

Cada endpoint suporta os seguintes métodos: `GET`, `POST`, `PUT`, `PATCH`, `DELETE`.



## Middlewares

A API utiliza os seguintes middlewares:

* `Morgan` - um middleware de logging.
* `express.json` - um middleware de body parser.
* `Routes` - middlewares de endpoint.
* `File not found` - um middleware para lidar com requisições para endpoints inexistentes.
* `Error handling` - um middleware para lidar com erros na API.

## Contribuidores
- [@Mateus Rayrisson](https://github.com/hassan9810)
- [@Arthur Oliveira]

## Conclusão

Esta API fornece uma solução completa para gerenciar uma clínica médica e pode ser usada como ponto de partida para futuras personalizações e expansões.
