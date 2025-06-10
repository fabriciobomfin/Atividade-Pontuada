# Atividade-Pontuada-2 atividade pontuada para ser entregue até dia 26/05/2025

Sistema de Gestão de Jogadores de Futebol ⚽
Este projeto é um sistema completo para gerenciar jogadores de futebol, permitindo o cadastro, a listagem e a visualização detalhada dos perfis dos jogadores. Ele foi desenvolvido com uma arquitetura dividida em frontend (React) e backend (Spring Boot), com persistência de dados em um banco de dados MySQL. 🚀

Funcionalidades ✨
O sistema oferece as seguintes funcionalidades principais:

Tela Inicial (Home): 🏠

Exibe o logo do time de futebol. 🥅

Serve como ponto de entrada do sistema.

Oferece um menu intuitivo para navegar para as telas de cadastro ou listagem de jogadores. ➡️

Tela de Cadastro de Jogador: ✍️

Permite o registro de novos jogadores com as seguintes informações:

Nome 👤

Sexo 🚻

Idade 🎂

Altura 📏

Peso ⚖️

Posição 🏟️

Número da camisa #️⃣

Os dados são enviados para o backend via API para persistência. 💾

Tela de Lista de Jogadores: 📋

Apresenta uma lista completa de todos os jogadores cadastrados.

Exibe informações chave como nome, posição e número da camisa.

Permite a visualização de detalhes específicos de cada jogador (funcionalidade opcional a ser implementada). 🔍

Estrutura de Dados do Jogador 📊
A estrutura de dados para cada jogador é a seguinte:

{
  "id": 1,
  "nome": "João da Silva",
  "sexo": "Masculino",
  "idade": 22,
  "altura": 1.80,
  "peso": 75,
  "posicao": "Atacante",
  "numeroCamisa": 10
}

Tecnologias Utilizadas 💻
Este projeto foi construído utilizando as seguintes tecnologias:

Frontend 🌐
React: ⚛️ Biblioteca JavaScript para construção de interfaces de usuário dinâmicas e reativas.

React Router DOM: 🛣️ Gerenciamento de rotas e navegação entre as diferentes páginas da aplicação.

Axios: 📡 Cliente HTTP baseado em Promises para fazer requisições a APIs externas.

Backend ⚙️
Spring Boot: 🍃 Framework Java para construção de aplicações robustas e escaláveis, ideal para o desenvolvimento de APIs RESTful.

MySQL: 🐘 Sistema de gerenciamento de banco de dados relacional para persistência dos dados dos jogadores.

Rotas da Aplicação (Frontend) 🗺️
O frontend utiliza as seguintes rotas:

/: Página Inicial (Home) 🏡

/cadastro: Tela de Cadastro de Jogador 📝

/jogadores: Tela de Lista de Jogadores 🧑‍🤝‍🧑

Exemplo de configuração de rotas:

import { BrowserRouter, Routes, Route } from "react-router-dom";
import Home from "./Home";
import CadastroJogador from "./CadastroJogador";
import ListaJogadores from "./ListaJogadores";

function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/cadastro" element={<CadastroJogador />} />
        <Route path="/jogadores" element={<ListaJogadores />} />
      </Routes>
    </BrowserRouter>
  );
}

Como Rodar o Projeto ▶️
Pré-requisitos ✅
Node.js e npm (para o frontend)

Java Development Kit (JDK) 8 ou superior (para o backend)

Maven ou Gradle (para o backend)

Servidor MySQL 🗃️

Configuração e Execução 🛠️
Backend (Spring Boot):

Clone este repositório. 📂

Navegue até a pasta do projeto backend.

Configure o banco de dados MySQL (application.properties ou application.yml para as credenciais e URL do banco). ⚙️

Execute a aplicação Spring Boot. 🚀

Frontend (React):

Navegue até a pasta do projeto frontend.

Instale as dependências: npm install 📦

Inicie a aplicação: npm start ⚡

A aplicação estará disponível em http://localhost:3000 (ou outra porta configurada). 🌐

Contribuição 👋
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests. 🤝

Licença 📜
Este projeto está licenciado sob a [Nome da Licença, ex: MIT License].
