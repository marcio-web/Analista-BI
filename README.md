# 📊 Desafio de BI - Painel Gerencial para E-commerce

## 📌 Sobre o Desafio
Este projeto consiste na criação de um painel gerencial para um e-commerce que deseja analisar suas vendas e traçar estratégias para impulsionar seus resultados. O painel deverá conter métricas relevantes para os analistas de negócios, permitindo uma visão clara do desempenho das vendas e do perfil dos clientes.

## 🎯 Objetivos
- Criar um dashboard com **duas páginas**: Visão de Clientes e Visão de Compras.
- Apresentar **métricas-chave** para análise de vendas e perfil dos clientes.
- Utilizar **storytelling** e um **layout atrativo** para facilitar a tomada de decisões.

## 📂 Bases de Dados
O desafio inclui duas bases:
1. **Base de Compras**
   - `idcompra`: Identificação da compra
   - `idcanalvenda`: Canal de venda
   - `bandeira`: Bandeira da compra
   - `data`: Data da compra
   - `preço`: Preço da compra
   - `preço_com_frete`: Preço da compra + frete
   - `nome_departamento`: Departamento do produto
   - `estado`: Estado da compra
   - `cliente_log`: Identificação do cliente

2. **Base de Clientes**
   - `cliente_log`: Identificação do cliente
   - `idade`: Idade do cliente
   - `uf_nascimento`: Estado de nascimento
   - `renda`: Renda do cliente

## 🏗️ Etapas de Desenvolvimento
### **1️⃣ Importação e Transformação dos Dados**
- Importação das bases no Power BI.
- Criação de uma coluna de **faixa de renda** para segmentação:
  - Até **R$ 1.750**
  - Até **R$ 2.500**
  - Até **R$ 5.000**
  - Até **R$ 7.500**
  - Até **R$ 10.000**

### **2️⃣ Criação de Páginas do Dashboard**
#### 📌 **Página 1: Visão de Clientes**
- **Gráficos e Métricas:**
  - **Cartões**: Quantidade de clientes, Média de renda dos clientes
  - **Gráficos de Barras**: Distribuição de idades, Distribuição de renda
  - **Filtros**: Idade, Faixa de renda, Estado de nascimento

#### 📌 **Página 2: Visão de Compras**
- **Gráficos e Métricas:**
  - **Cartões**: Quantidade total de vendas, Valor total de vendas sem frete, Valor total de vendas com frete
  - **Gráficos de Linhas**: Contagem de vendas por mês, Valor total de vendas por mês
  - **Gráficos de Barras**: Quantidade de vendas por categoria, Valor total de vendas por categoria
  - **Filtros**: Bandeira, Estado, Canal de venda, Departamento

## 📈 Métricas Criadas
- **KPIs em Cartões:**
  - Quantidade total de vendas
  - Valor total de vendas sem frete
  - Valor total de vendas com frete
  - Quantidade total de clientes
  - Média de renda dos clientes

- **Gráficos de Linhas:**
  - Contagem de vendas por mês
  - Valor total de vendas por mês

- **Gráficos de Barras:**
  - Quantidade de vendas por categoria
  - Valor total de vendas por categoria
  - Distribuição de idades dos clientes
  - Distribuição de renda dos clientes

- **Filtros:**
  - Bandeira, Estado, Canal de venda, Departamento, Idade, Faixa de renda, Estado de nascimento

## 📸 Visão dos Dashboards

**🔹 Página 1 - Visão de Vends**  
🖼️ ![Visão de Vendas](./imagens/visao-vendas.png)

**🔹 Página 2 - Visão de Clientes**  
🖼️ ![Visão de Clientes](./imagens/visao-clientes.png)

## 🚀 Conclusão
Este painel permitirá que a equipe de negócios compreenda melhor o comportamento de compra dos clientes, identifique oportunidades de crescimento e otimize as estratégias para aumentar o faturamento do e-commerce. A combinação de métricas detalhadas, filtros interativos e um design intuitivo garantirá uma análise eficiente e tomada de decisão baseada em dados.

🔗 **Tecnologias utilizadas**: Power BI, DAX, Modelagem de Dados, Visualizações Interativas.
