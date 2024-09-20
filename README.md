# Back-End
>O back-end se refere à parte do desenvolvimento de software que lida com a lógica de aplicação, gerenciamento de dados e integração com o servidor. Enquanto o front-end é responsável pela interface que o usuário interage, o back-end é onde toda a magia acontece, garantindo que tudo funcione nos bastidores. Os desenvolvedores de back-end criam e mantêm a arquitetura que suporta a aplicação, trabalhando com bancos de dados, APIs e servidores.

# Node.js:
>Node.js é um ambiente de execução JavaScript que permite executar código JavaScript no lado do servidor. Criado em 2009, ele usa o mecanismo V8 do Google Chrome para compilar JavaScript em código de máquina, tornando-o extremamente eficiente e rápido.

## Instalar o Node.js no seu computador:
* Pesquise no navegador node.js.org e aperte em instalar na versão do seu computador;

## Inicializando o projeto:
### Primeiros passos:
* Criar pasta;
* Abrir o cmd : Desktop; cd + (Nome da pasta) ; 
* Abrir Vs code: apt.js ; 
* Abrir cmd : apt.js;
* Cmd ; node + (nome do arquivo);

### Dentro do terminal do Vs Code escreva:
* npm init -y 
* npm install express

### Configure o servidor:
* const express = require('express'); 
* const app = express(); 
* app.use(express.json()) 
* app.get('/', (req, res) => { 
* res.json({ msg:”Olá” }); 
* }); 
* app.listen(3000); 

### Execute o servidor:
#### Dentro do terminal do Vs Code escreva:
* node app.js 
### Abra o navegador e escreva :
* localhost:3000

# API :

> Uma API (Interface de Programação de Aplicações) é um conjunto de regras que permite que diferentes softwares se comuniquem. Ela funciona como uma ponte, facilitando a troca de informações entre sistemas. Existem vários tipos de APIs, como públicas, privadas e de parceiros. As APIs oferecem diversas vantagens, incluindo integração facilitada, reutilização de funcionalidades e escalabilidade, sendo essenciais para o desenvolvimento de aplicações modernas e interconectadas.

# Conexão MySql:

> O mysql2 é uma biblioteca popular para Node.js que permite interagir com bancos de dados MySQL. É uma alternativa ao pacote mysql e oferece suporte a várias funcionalidades avançadas, como:

## Principais Características
* Promessas e Async/Await: O mysql2 suporta Promises, o que facilita o uso de async/await, tornando o código mais limpo e legível.
* Performance: É otimizado para alta performance e pode lidar com conexões em massa de forma eficiente.
* Suporte a Prepared Statements: Permite executar consultas de forma segura, evitando injeções de SQL.

## Como usar:

### Para começar a usar o mysql2, você pode instalá-lo via npm:
* npm install mysql2

## Um exemplo básico de como conectar a um banco de dados e fazer uma consulta seria:

* const mysql = require('mysql2/promise');
* async function main() {
* const connection = await mysql.createConnection({host: 'localhost', user: 'root', database: 'test'});
* const [rows] = await connection.execute('SELECT * FROM users');
* console.log(rows);
* await connection.end();
* }
*main().catch(console.error);











