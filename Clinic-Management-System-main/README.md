# Sistema de Gestão de Clínicas
Sistema de Gestão de Clínicas - API REST para gerenciar uma clinica local 

## Tecnologias Utilizadas no Beck-end

Neste projeto foram utilizadas as seguintes tecnologias e bibliotecas:

- **Node.js**: Ambiente de execução JavaScript no servidor.
- **Express**: Framework para criação de servidores web e APIs.
- **CORS**: Middleware para habilitar o compartilhamento de recursos entre diferentes origens.
- **Prisma**: ORM para acesso e manipulação de banco de dados com TypeScript/JavaScript.
- **Insomnia** Para testes 

## Tecnologias Utilizadas no Front-end

Neste projeto foram utilizadas as seguintes tecnologias e bibliotecas:

- **React**: Biblioteca para construção de interfaces de usuário.
- **React Hooks** (`useState`, `useEffect`, `useRef`): Para gerenciamento de estado, efeitos colaterais e referências.
- **CSS**: Para estilização dos componentes (importado via `./style.css`).
- **Axios **: Biblioteca para requisições HTTP (no código importada como `api`).
- **Importação de imagens**: Gerenciamento de assets estáticos, como ícones (`Trash.png`).

## Arquitetura do Projeto

### Backend

O backend foi desenvolvido utilizando uma arquitetura monolítica simples baseada em API REST. As principais características são:

- **Monolítica:** O servidor Express gerencia todas as rotas, lógica de negócio e acesso ao banco de dados em uma única camada.
- **API REST:** Implementação de rotas para operações CRUD (`POST`, `GET`, `PUT`, `DELETE`) sobre a entidade `usuarios`.
- **ORM Prisma:** Utilização do Prisma Client para interação direta com o banco de dados, facilitando consultas e manipulações.
- **Middleware básico:** Uso de `express.json()` para parsing de JSON e `cors()` para habilitar requisições cross-origin.
- **Sem separação explícita de camadas:** Toda a lógica está centralizada, sem divisão formal em controllers, services ou repositories.

Essa arquitetura é simples, fácil de entender e ideal para aplicações pequenas ou protótipos rápidos.

---

### Frontend

O frontend foi desenvolvido com React utilizando uma arquitetura funcional simples. As principais características são:

- **Componente único:** Toda a aplicação está dentro de um único componente funcional (`Home`), que gerencia estado, efeitos e renderização.
- **React Hooks:** Uso de `useState`, `useEffect` e `useRef` para controle de estado local, efeitos colaterais e referências a elementos do DOM.
- **Gerenciamento local de estado:** O estado da aplicação (lista de usuários, edição, visibilidade) é mantido dentro do componente.
- **Chamada direta à API:** Funções para criação, leitura, atualização e exclusão de dados são feitas diretamente no componente.
- **Estilização externa:** Arquivo CSS separado para estilos visuais.
- **Importação de assets:** Uso de imagens estáticas para botões e ícones.

Essa abordagem é adequada para projetos pequenos ou MVPs, mas pode demandar refatoração para escalabilidade em aplicações maiores.

---


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
- [insomnia]

## Configuração

A API usa as seguintes variáveis de ambiente:

* `PORT` - a porta na qual a API vai escutar por requisições.
* `MONGODB_URI` - a URL do banco de dados MongoDB para conectar.
* `MONGODB_LOCAL` - a URL do banco de dados MongoDB local para conectar.


## Instalação
Para instalar a plataforma e suas dependências, siga os seguintes passos:

## Funcionalidades

O projeto possui diversas funcionalidades, incluindo:

- Cadastrar pacientes: Permite que pacientes se cadastrem no centro médico.
- Autenticar usuários: Permite que usuários se autentiquem no centro médico.
- Gerenciar consultas: Permite que usuários gerenciem consultas, incluindo adicionar consultas, obter todas as consultas e mais.



## Contribuidores
- [@Mateus Rayrisson](https://github.com/ElMateus333)
- [@Arthur Oliveira]

## Conclusão

Esta API fornece uma solução completa para gerenciar uma clínica médica e pode ser usada como ponto de partida para futuras personalizações e expansões.
