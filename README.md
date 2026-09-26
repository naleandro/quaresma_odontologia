Sistema de Gerenciamento Petshop
-------------------------
📋 Sobre o Projeto
-----------------------
Este projeto foi desenvolvido como requisito para a disciplina do Projeto Prático 
de Programação da Universidade Nove de Julho (UNINOVE).

O sistema consiste em uma aplicação Web focada no gerenciamento 
de um Petshop, contando com um sistema de controle de acesso (login) e um CRUD 
(Create, Read, Update, Delete) completo e funcional. A arquitetura foi pensada 
de forma essencialista, garantindo que as operações de banco de dados e a 
interface do usuário operem de forma simples e direta.

🚀 Funcionalidades
----------------------
O sistema atende aos seguintes requisitos:

Autenticação: Validação de login e senha para acesso seguro ao painel.
Cadastrar: Inclusão de novos animais de estimação com dados como raça, nome, idade, características e dono.
Listar (Leitura): Exibição de todos os registros cadastrados na tela do site.
Alterar (Update): Atualização de dados de animais de estimação já cadastrados no banco.
Excluir (Excluir): Remoção de registros do sistema.

📷 Telas da Aplicação
----------------------------
🔐 Tela de Login
<img width="1365" height="645" alt="login" src="https://github.com/user-attachments/assets/cd98bad0-e2ce-48a8-a4be-6bd01eb7f3a1" />

📊 Painel Administrativo
<img width="1365" height="647" alt="dashboard" src="https://github.com/user-attachments/assets/7779fca4-fb08-4cb1-9ccc-dde933d27aa2" />

🐾 Cadastro de Novos Pets
<img width="1365" height="643" alt="cadastro" src="https://github.com/user-attachments/assets/319eacf5-a81c-4083-9dc6-91239474e71b" />

📑 Listagem e Gerenciamento de Pets (CRUD)
<img width="1365" height="641" alt="listagem" src="https://github.com/user-attachments/assets/6573bb2b-c329-45c7-86dc-ad75cb1e0430" />

🛠️ Tecnologias e Ferramentas
---------------------------------------
Linguagem: Java (Web)
IDE: Apache NetBeans
Servidor: Apache Tomcat
Banco de Dados: MySQL
DevOps & Gestão: Controle de versão via GitHub e gerenciamento de tarefas via Kanban (Trello).

🗄️ Banco de Dados
---------------------------

O sistema utiliza um banco de dados relacional chamado db_petshop contendo 
duas tabelas 
1. usuarios: Responsável por armazenar as credenciais de acesso ao sistema.
2.pet: Responsável por armazenar as informações obrigatórias do negócio.

💡 Nota: O script SQL completo para a criação do banco de dados e
inserção do usuário administrador padrão (admin/123456) está disponível no arquivo script_banco.sqlna raiz deste repositório.

⚙️ Como executar o projeto localmente
--------------------------------------
1.Clonar o:
git clone [https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git](https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git)

2.Configuração do Banco de Dados:
Execute o arquivo script_banco.sqlno seu MySQL Workbench para 
criar a estrutura necessária.

Atenção: Por questões de segurança, as senhas de conexão foram 
omitidas no código. Você deve abrir os arquivos .jspque fazem 
conexão com o banco e inserir suas credenciais locais na linha: 
DriverManager.getConnection("jdbc:mysql://localhost:3306/db_petshop", "root", "SUA_SENHA_AQUI");

3)Arquivos que exigem ajuste de senha:
acesso.jsp, salvar_usuario.jsp, salvar_pet.jsp, listar_pets.jsp,
editar_pet.jsp, atualizar_pet.jspe excluir_pet.jsp.
