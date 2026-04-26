# Projeto de Integração de Microsoft Azure com Microsoft Power BI
Projeto da DIO de Integração do Microsoft Azure com o Power BI.
## 🎯 Objetivo
Criar uma relatório no Power BI utilizando **Azure MySQL**, realizando o tratamento, transformação e modelagem da base de dados.

---

# 🧩 Etapas do Projeto

## 1️⃣ Criar instância MySQL no Azure
1. Acesse o Portal Azure → https://portal.azure.com  
2. Clique em **Create a resource**
3. Pesquise por **Azure Database for MySQL**
4. Clique em **Create**

### Configurações básicas
- Resource Group: criar novo ou usar existente  
- Server Name: `desafio-azure-projeto`  
- Region: escolher a mais próxima  
- Workload type: **Development**  
- Authentication: usuário + senha  

5. Clique em **Review + Create**
6. Após criação, acessar:
   - **Networking → Firewall rules**
   - Habilitar:
     - Allow public access
     - Add current client IP

---

## 2️⃣ Criar o Banco de Dados a partir do GitHub

### 2.1 Conectar ao MySQL
Ferramentas possíveis:
- MySQL Workbench  
- Azure Cloud Shell  
- DBeaver  

### 2.2 Criar banco

---

## 3️⃣ Conectar Power BI ao MySQL no Azure

### 3.1 Instalar pré-requisitos
Antes de conectar o Power BI ao MySQL, instalar:

- MySQL Connector/NET

Download:
https://dev.mysql.com/downloads/connector/net/

### 3.2 Conectar o Power BI ao banco MySQL

1. Abrir o **Power BI Desktop**

2. Clique em:
Obter Dados → MySQL Database

3. Preencher as credenciais de acesso

4. Importar os dados

5. Selecionar todas as tabelas do banco.

6. Clique em **Transform Data** para abrir o Power Query.

---

## 4️⃣ Transformação de Dados (Power Query)

Todas as etapas abaixo foram realizadas no **Power Query Editor**.

### 4.1 Verificação de Cabeçalhos e Tipos de Dados
Conferir nomes das colunas e ajustar tipos.

### 4.2 Escolher as colunas que serão usadas
Selecionar as colunas que será trabalhadas.

