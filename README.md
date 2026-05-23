### 🎬 Mynetflox

Sistema de banco de dados relacional desenvolvido para uma plataforma de streaming de filmes e séries, utilizando MySQL e modelagem DER no MySQL Workbench.

### 📚 Sobre o Projeto

O projeto Mynetflox foi criado com o objetivo de simular a estrutura de um serviço de streaming sob demanda, permitindo o gerenciamento de:

Usuários
Endereços
Conteúdos
Estúdios
Histórico de visualização

O banco foi modelado seguindo regras de relacionamento e normalização para garantir organização, integridade e escalabilidade dos dados.

🗂 Estrutura do Banco de Dados
# 👤 Usuário

Responsável pelo cadastro dos clientes da plataforma.

Campos:
ID
Nome
Email
CPF
Endereço (FK)
# 📍 Endereço

Armazena os dados de localização do usuário.

Campos:
ID
Rua
Número
Cidade
Estado
CEP
# 🎥 Conteúdo

Tabela responsável pelos filmes e séries cadastrados.

Campos:
ID
Título
Gênero
Ano
Estúdio (FK)
# 🏢 Estúdio

Representa os estúdios produtores dos conteúdos.

Campos:
ID
Nome
# ▶️ Visualização

Tabela intermediária responsável pelo relacionamento entre usuários e conteúdos assistidos.

Campos:
ID
Usuário (FK)
Conteúdo (FK)
Tempo de Visualização
# 🔗 Relacionamentos
Relacionamento	Tipo
Usuário → Endereço	1:1
Estúdio → Conteúdo	1:N
Usuário ↔ Conteúdo	N:N
# 🛠 Tecnologias Utilizadas
MySQL
MySQL Workbench
SQL
DER (Diagrama Entidade-Relacionamento)
# 📌 Objetivos do Projeto
Praticar modelagem de banco de dados
Aprender relacionamentos entre tabelas
Utilizar chaves primárias e estrangeiras
Desenvolver lógica de estruturação relacional
Simular um sistema real de streaming
# 🚀 Futuras Melhorias
Sistema de assinaturas
Controle de planos
Sistema de avaliações
Favoritos
Histórico completo de reprodução
Controle de episódios e temporadas
### 📷 Diagrama ER

![DER do Projeto](<img width="955" height="427" alt="Captura de tela 2026-05-22 212311" src="https://github.com/user-attachments/assets/6145413b-8b1a-45bf-b9d5-4da75ab5f085" />
)
## ⚖️ Licença

Este projeto está sob a licença MIT.

## 👨‍💻 Autor

Samuel Covalski
Estudante de Desenvolvimento Full Stack
SENAI • SENAC • DIO
