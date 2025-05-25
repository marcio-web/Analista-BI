 # 📊 Dashboard de Aquisição de Leads - EdTech

## 📌 Contexto

Como analista de dados de uma empresa EdTech, seu principal objetivo é **impulsionar o crescimento da base de usuários** da plataforma. O foco está em compreender o comportamento dos leads, sua origem, engajamento com as demonstrações e etapas do funil de conversão.

Este dashboard foi desenvolvido para oferecer **insights práticos e visuais**, permitindo que os times de negócios e marketing tomem decisões baseadas em dados.

---

## 🔧 Ferramentas Utilizadas

* **Metabase** (plataforma de BI)
* **SQL** para manipulação e agregação de dados
* **Fonte de dados**: Tabelas relacionais do banco

---

## 🎯 Objetivos do Dashboard

* Analisar o perfil dos leads (idade, gênero, escolaridade)
* Avaliar canais de aquisição de usuários
* Observar o engajamento com as demonstrações
* Acompanhar o volume de ligações bem-sucedidas por plataforma
* Gerar base para ações de marketing e vendas

---

## 📈 Painéis do Dashboard

### 🟢 1) **Distribuição por Gênero**

**Tipo de Gráfico:** Pizza
**Tabela:** `leads_basic_details`
**Objetivo:** Visualizar a proporção de leads masculinos e femininos.

**SQL Usado:**

```sql
SELECT
  Gender,
  COUNT(*) AS quantidade
FROM
   leads_basic_details
GROUP BY
  Gender
ORDER BY
  quantidade DESC;

```

---

### 🔢 2) **Média de Idade**

**Tipo de Gráfico:** Cartão
**Tabela:** `leads_basic_details`
**Objetivo:** Obter a média de idade dos leads.

**SQL Usado:**

```sql
SELECT
  AVG(Age) AS media_idade
FROM
  leads_basic_details;
```

---

### 📚 3) **Quantidade de Leads por Grau de Escolaridade**

**Tipo de Gráfico:** Barras
**Tabela:** `leads_basic_details`
**Objetivo:** Entender o nível educacional predominante dos leads.

**SQL Usado:**

```sql
SELECT
  current_education,
  COUNT(*) AS quantidade
FROM
  leads_basic_details
GROUP BY
  current_education
ORDER BY
  quantidade;
```

---

### 🌐 4) **Média de Porcentagem Assistida da Demonstração por Idioma**

**Tipo de Gráfico:** Tabela
**Tabela:** `leads_demo_watched_details`
**Objetivo:** Avaliar o engajamento dos leads com as demonstrações, filtrando apenas os que assistiram mais de 50%.

**SQL Usado:**

```sql
SELECT 
    language,
    AVG(watched_percentage) AS average_watched_percentage
FROM 
    leads_demo_watched_details
WHERE 
    watched_percentage > 0.5
GROUP BY 
    language
ORDER BY 
    average_watched_percentage DESC;

---

### 📞 5) **Quantidade de Ligações Atendidas por Plataforma ao Longo do Tempo**

**Tipo de Gráfico:** Linhas
**Tabelas:** `leads_basic_details`, `leads_interaction_details`
**Objetivo:** Acompanhar os canais mais eficazes em gerar leads que atendem ligações ao longo do tempo.

**SQL Usado:**

```sql
SELECT
    DATE(i.call_done_date) AS call_date,
    l.lead_gen_source AS platform,
    COUNT(*) AS total_calls
FROM leads_basic_details l
JOIN leads_interaction_details i
  ON l.lead_id = i.lead_id
WHERE i.call_status = 'successful'
GROUP BY
    DATE(i.call_done_date),
    l.lead_gen_source
ORDER BY call_date, platform;

```
## 📊 **Visualização do Dashboard**  

<p align="center">
  <img src="./imagens/dash.webp" width="500px">
</p> 
---

## 📍 Considerações Finais

Este dashboard oferece uma **visão abrangente do funil de aquisição de leads**, desde a origem até o comportamento em chamadas e demonstrações. Os dados orientam **ações estratégicas** de marketing e vendas, com o objetivo de:

* **Aumentar a taxa de conversão**
* **Direcionar recursos para canais mais eficazes**
* **Melhorar o conteúdo e formato das demonstrações**
* **Segmentar campanhas conforme perfil dos leads**

---

Se desejar, posso montar o layout visual em wireframe ou sugerir filtros e interações adicionais para o dashboard. Deseja isso?
                                                 


