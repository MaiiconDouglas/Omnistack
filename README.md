# Be The Hero - Semana OmniStack 11

Projeto desenvolvido na semana OmniStack 11 da [Rocketseat](https://rocketseat.com.br/) dias 23/03/2020 à 27/03/2020.

Com as aulas online com o  Diego Fernandes.

O projeto ensinado encontra-se [Aguardando a Rocketseat disponibilizar o repositório]
  
## Projeto

Criar uma plataforma web/mobile utilizando *React* e *React-native* para frontend da web e mobile respectivamente e utilizar *Express* para o backend.
 
### Tecnologias utilizadas

```
git, node, express, knex, sqlite, reactjs, react-native, expo
```

### Instalação

Clone o repositório, utilizando **git clone** ou faça o **download** do repositório.

----

Após clonar ou baixar o repositório instale as dependências necessárias:

Utilize o **npm** para instalar as dependências nas pastas *backend*, *react-frontend*, *vue-frontend*, *mobile*.

```
npm install
```
Após instalar as dependências você precisa rodar o comando do knex para criar o banco de dados SQLite e as rodar as migrações. 

```
npx knex migrate:latest
```

Após a geração do banco de dados e das migrações você poderá rodar o backend, frontend e mobile utilizando

**Para o backend e react-frontend:**
```
npm start
```

**Para o mobile**
```
expo start
```
**Pacotes usados**
```
npm init -y
npm install express
npm install nodemon -D
npm install sqlite3
npm install knex 
npm install react-router-dom

npx knex migrate:make create_

```

**React-Icons**
```
npm install react-icons // tem todos os pacotes de icones existente 
```

Para visualização da aplicação mobile utilize o celular com o aplicativo *Expo* ou emulador Android/iOS.


## Mudanças

//Em breve

#### Backend - Express

  * Banco de dados mantive o campo **id** do SQL intacto e adicionei um campo **key** para ser usado como identificado das ONGs
  * Adicionei os **testes** ao backend (**atualizado com teste jwt**)
  * Adicionei a pasta **http** com *REST requests* para rodar no **vscode** usando o pacote **Rest Client** caso não queira utilizar *insomnia* ou *postman*

#### ReactJS - Frontend

  * Adicionei uma janela de confirmação de cadastro de nova ONG no *frontend*.
```
RegisterSuccess
```
  * Adicionado **paginação** no perfil da ONG frontend.
  * Adicionado página de **edição** de ONG
```
Account
```
  * Adicionado botão de **apagar conta** na página de edição da ONG
  * Adicionado alertas de confirmação de conta atualizada na página de perfil e de conta apagada na página inicial
  * Adicionado página para **atualizar** caso
```
EditIncident
```
  * Removi o campo **KEY** da tabela **ongs**
  * Adicionei os timestamps **created_at** e **updated_at** às tabelas **ongs** e **incidents**
  * Adicionado autenticação com **JWT**
  * Adicionado **envio de e-mail** após o cadastro
  * Armazenamento do **token JWT** utilizando cookie **httpOnly**
  * *(em breve)* adicionar **Redux** para lidar com as states

#### React Native - Mobile

  * Adicionei funções de refresh do **FlatList** no mobile para exibir o carregamento de novos casos:
```
onRefresh={loadIncidents}
refreshing={loading}
```
  * Se não tiver nenhum caso para exibir fará requisição para listar casos a cada **6** segundos

## Autor

**Maicon Douglas** 
* [Github](https://github.com/MaiiconDouglas/)
* [Discord] - Maicon Douglas#1385
* [linkedin](https://www.linkedin.com/in/maiconndouglas/)

## Agradecimentos

* Rocketseat
* Diego Fernandes
