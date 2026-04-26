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

---


### 5️⃣ Criação de Visuais de Relatório

- **Gráfico de Barras – Top Salários**
  - Exibe os funcionários com os maiores salários máximos.
  - Permite identificar rapidamente posições ou colaboradores com maior custo salarial.

- **Gráfico de Área – Empregados por Gerente**
  - Mostra a quantidade de empregados sob responsabilidade de cada gerente.
  - Auxilia na análise de carga de gestão e distribuição de equipes.

- **Gráfico Radar – Empregados por Departamento**
  - Apresenta a contagem de empregados por departamento.
  - Facilita a comparação do tamanho relativo das áreas da empresa.

- **Gráfico de Pizza – Empregados por Sexo**
  - Exibe a distribuição percentual dos empregados por sexo.
  - Fornece uma visão geral da composição demográfica da organização.

- **Gráfico de Colunas – Dependentes por Funcionário**
  - Mostra a quantidade máxima de dependentes associados a cada funcionário.
  - Apoia análises relacionadas a benefícios e encargos adicionais.

---

## 🏆 Projeto

- [Projeto - Integração Azure e Power BI](https://github.com/guimazza-ai/projeto-relatorio-gerencial-vendas/blob/main/Projeto/Projeto_Relatorio%20Gerencial%20de%20Vendas.pbix)
- [Base de Dados - Azure_company](https://github.com/guimazza-ai/projeto-relatorio-gerencial-vendas/blob/main/Projeto/Financial%20Sample.xlsx)
- [Apresentação - Relatório de Gerenciamento de Empregados](https://github.com/guimazza-ai/projeto-relatorio-gerencial-vendas/blob/main/Projeto/Apresenta%C3%A7%C3%A3o_Relat%C3%B3rio%20Gerencial%20de%20Vendas.pptx)
