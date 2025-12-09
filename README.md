# 🚀 CEIControl - Sistema de Gestão para Centros de Educação Infantil Públicos

![Capa do Projeto](https://placehold.co/800x200/2E8B57/FFFFFF?text=CEIControl+-+Sistema+Web+para+CEIs)

O **CEIControl** é uma plataforma web desenvolvida para simplificar e modernizar a gestão de Centros de Educação Infantil (CEIs) públicos. Nosso objetivo é centralizar em um único sistema o cadastro de usuários, gestão de recursos, agenda digital e o canal de comunicação direta entre a coordenação e os responsáveis pelos alunos.

O projeto é uma iniciativa da empresa JEM Tech, voltada para o desenvolvimento de soluções digitais de gestão para o setor público.

| Autores | Faculdade |
| :--- | :--- |
| Eduardo Ferreira Martins | Faculdade de Tecnologia de Ferraz de Vasconcelos (FATEC) |
| João Vitor Martins Silva | Curso Superior de Análise e Desenvolvimento de Sistemas |

---

## 🌟 Funcionalidades Principais

O sistema oferece autenticação multi-perfil (Admin, Professor e Responsável) e centraliza as ferramentas essenciais:

* **Gestão de Cadastros (CRUD):** Gerenciamento completo (Cadastro, Consulta, Edição, Exclusão) de Fornecedores, Produtos e Serviços.
* **Comunicação Integrada:** Chat em tempo real e envio de comunicados com fluxo de aprovação.
* **Agenda Digital Inteligente:** Registro de eventos, datas importantes e reuniões, compartilhada entre coordenação e responsáveis.
* **Gestão Pedagógica:** Módulos para **Registro de Ocorrências** e **Geração de Relatórios**.
* **Acesso Controlado:** O sistema deve validar o perfil de usuário em cada requisição, impedindo acessos indevidos (RNF04).

## 💻 Tecnologias Adotadas

O CEIControl é construído com foco em linguagens de código aberto (Open Source) e segue um modelo de arquitetura Cliente-Servidor.

| Categoria | Tecnologia | Uso |
| :--- | :--- | :--- |
| **Back-end** | PHP | Linguagem de programação principal. |
| **Banco de Dados** | MySQL | Sistema Gerenciador de Banco de Dados Relacional (SGBDR). |
| **Front-end** | HTML5, CSS3, JavaScript | Estrutura de interface e estilo, com foco em responsividade e usabilidade. |
| **Arquitetura** | Cliente-Servidor, Cloud (Nuven) | O sistema é acessado via Navegador e hospedado em Serviço de Nuvem. |

---

## 🛠️ Instalação e Configuração

Para rodar o CEIControl localmente, você precisa de um ambiente de servidor web com suporte a PHP e MySQL (como XAMPP, WAMP ou MAMP).

### 1. Clonar o Repositório

No seu terminal, clone este projeto para o diretório `htdocs` do seu XAMPP (ou similar):

```bash
git clone [https://github.com/EduardoMartins-tech/CEIControl-Alpha.git](https://github.com/EduardoMartins-tech/CEIControl-Alpha.git)
cd CEIControl-Alpha


2. Configuração do Ambiente e Acesso
Crie o Banco de Dados: Acesse o phpMyAdmin (http://localhost/phpmyadmin/) e crie um novo banco de dados (Ex: ceicontrol_db).

Importe as Estruturas: Utilize os scripts SQL fornecidos no projeto para criar as tabelas e popular os dados de teste.

# Cria a estrutura das tabelas
mysql -u [seu_usuario] -p ceicontrol_db < tabelas.sql
# Adiciona dados de teste
mysql -u [seu_usuario] -p ceicontrol_db < dados_de_teste.sql

3. Ajuste a Conexão: Localize e edite o arquivo de conexão (provavelmente database.php) para informar as credenciais do seu banco de dados local:

hostname: localhost

username: (Ex: root para XAMPP)

password: (Ex: vazio para XAMPP)

database: ceicontrol_db

4. Acesse o Sistema: Após iniciar o servidor Apache e o MySQL, o sistema estará acessível no seu navegador:

http://localhost/CEIControl-Alpha/index.html
