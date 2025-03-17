# 📊 **Desafio de BI - Painel Gerencial para Marketing Digital**  

## 📌 **Sobre o Desafio**  
Este projeto consiste na criação de um **painel gerencial para uma empresa de marketing digital** que deseja acompanhar seu desempenho e otimizar suas estratégias para alcançar suas metas trimestrais. O painel fornecerá insights essenciais para a equipe de gestão, permitindo uma **tomada de decisão baseada em dados**.  

## 🎯 **Objetivos**  
- Criar um **dashboard interativo** no Power BI com **duas páginas**: Visão Geral e Detalhamento.  
- Apresentar **KPIs estratégicos** para análise de desempenho das campanhas.  
- Utilizar **storytelling** e um **layout visualmente intuitivo** para facilitar a interpretação dos dados.  

## 📂 **Bases de Dados**  
A base de dados utilizada contém informações sobre **o desempenho das campanhas em março de 2023**, incluindo receitas, compradores, visualizações e segmentações.  

### **📌 Estrutura dos Dados**  
| **Coluna** | **Descrição** |
|------------|--------------|
| **Data** | Data do período analisado |
| **Receita Total** | Receita total por dia |
| **Receita Média por Compra** | Valor médio gasto por cliente |
| **Total de Compradores** | Número de clientes que realizaram compras |
| **Visualizações** | Número total de acessos ao site |
| **Compradores por Origem** | Quantidade de clientes por canal de aquisição |
| **Usuários Ativos por Plataforma** | Segmentação por tipo de dispositivo utilizado |
| **Usuários por Cidade** | Quantidade de usuários por localização |
| **Usuários Ativos por Gênero** | Distribuição de clientes por gênero |

---

## 🏗️ **Etapas de Desenvolvimento**  

### **1️⃣ Importação e Transformação dos Dados**  
- Importação dos dados no **Power BI**.  
- Criação de **colunas calculadas**, incluindo **% de visualização** (Visualizações / Usuários Ativos).  

### **2️⃣ Criação de Páginas do Dashboard**  

#### 📌 **Página 1: Visão Geral**  
**Objetivo:** Apresentar os principais indicadores de forma clara e objetiva.  

- **KPIs em Cartões:**  
  - Receita Total  
  - Soma da Receita Média por Compra  
  - Total de Compradores  
  - Total de Visualizações  

- **Gráficos:**  
  - **Gráficos de Pizza:** Usuários Ativos por Gênero, Usuários Ativos por Plataforma.  
  - **Gráficos de Barras:** Compradores por Origem, Usuários por Cidade.  
  - **Gráficos de Linhas:** Evolução de Compradores por Data, Evolução da % de Visualização.  

#### 📌 **Página 2: Detalhamento**  
**Objetivo:** Permitir uma análise aprofundada das métricas e segmentações.  

- **KPIs em Cartões:**  
  - Receita Média por Compra  
  - Total de Compradores por Plataforma  
  - Comparação de Visualizações vs. Compradores  

- **Filtros Interativos:**  
  - Período de Análise  
  - Plataforma  
  - Cidade  
  - Origem dos Compradores  

---

## 📊 **Visualização do Dashboard**  
<p align="center">
  <img src="./imagens/visao-geral.png" width="500px">
  <img src="./imagens/detalhamento.png" width="500px">
</p> 

---

## 📈 **Métricas Criadas**  

- **KPIs Estratégicos:**  
  - Receita Total  
  - Receita Média por Compra  
  - Total de Compradores  
  - Total de Visualizações  

- **Gráficos Dinâmicos:**  
  - Evolução de Compradores ao longo do tempo  
  - Comparação entre origens de tráfego  
  - Segmentação de usuários por cidade e plataforma  

- **Filtros Interativos:**  
  - Data, Gênero, Plataforma, Localização  

---

## 🎨 **Storytelling e Layout**  
- Uso de **cores estratégicas** para facilitar a interpretação.  
- **Posicionamento otimizado** dos gráficos para melhor usabilidade.  
- **Dicas visuais** para guiar a análise dos dados.  
- Interatividade para permitir **exploração flexível das métricas**.  

---

## 🚀 **Conclusão**  
Este painel permite que a equipe de marketing tome **decisões baseadas em dados**, otimizando campanhas e melhorando o desempenho geral. A combinação de **KPIs detalhados, segmentações interativas e visualizações impactantes** garante uma análise eficiente e prática.  

🔗 **Tecnologias utilizadas:** Power BI, DAX, Modelagem de Dados, Storytelling com Dados.  

📢 **Próximos Passos:** Implementação de **análises preditivas** para otimizar ainda mais as campanhas de marketing.  