# 🏢 Sistema de Gerenciamento de RH (RH System)

O **Sistema de RH** é uma aplicação desenvolvida em **Java** com persistência de dados em banco de dados relacional (**MySQL**). O sistema foi projetado para otimizar e automatizar rotinas do setor de Recursos Humanos, oferecendo uma solução robusta para o gerenciamento de dados corporativos.

---

### 🛠️ Tecnologias e Ferramentas Utilizadas

- **Linguagem Principal:** Java (JDK 8+)
- **Banco de Dados:** MySQL
- **Linguagem de Consulta:** SQL
- **Conectividade:** JDBC (*Java Database Connectivity*)

---

### 📌 Principais Funcionalidades

- **Módulo de Conexão Segura:** Integração com o banco de dados `projeto_final` utilizando o driver JDBC e tratamento adequado de fusos horários (`UTC`).
- **Gestão de Exceções:** Mapeamento e tratamento de falhas de conexão e consultas SQL (`SQLException` e `ClassCastException`) para maior estabilidade da aplicação.
- **Gerenciamento de Recursos:** Encerramento apropriado e seguro de conexões ativas com o banco para evitar vazamento de memória.

---

### 🗄️ Estrutura e Configuração do Banco de Dados

A aplicação conecta-se ao servidor local MySQL na porta padrão `3306`.

#### Configurações de Conexão:
- **URL JDBC:** `jdbc:mysql://localhost:3306/projeto_final?useTimezone=true&serverTimezone=UTC`
- **Banco de Dados:** `projeto_final`

> 💡 **Nota de Segurança:** Certifique-se de configurar suas credenciais do MySQL (usuário e senha) no arquivo `ConexaoBanco.java` ou utilizar variáveis de ambiente antes de executar a aplicação localmente.

---

### 🚀 Como Executar o Projeto Localmente

#### Pré-requisitos:
- [Java JDK](https://www.oracle.com/java/technologies/downloads/) instalado na máquina.
- Servidor [MySQL](https://www.mysql.com/) rodando localmente.
- Driver JDBC do MySQL (`mysql-connector-java.jar`) adicionado às dependências do projeto.

#### Passos para execução:

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
