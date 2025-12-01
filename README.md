# Projeto de Pré-Processamento e Análise Exploratória dos Dados Olist

## 👥 Integrantes
- Marcelo Sampaio de Sousa


---

## 🔗 Base de Dados Utilizada
Os datasets utilizados pertencem à base pública da Olist, disponível em:  
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

---

## 🎯 Objetivo do Projeto
O objetivo deste projeto é aplicar todas as etapas do pré-processamento e da análise exploratória de dados (EDA) utilizando a base Olist.  
O trabalho envolve integração dos datasets, limpeza, padronização, tratamento de outliers e nulos, conversão de tipos, criação de novos atributos e geração de visualizações para compreensão dos padrões logísticos.

---

## 🧹 Descrição do Processo de Tratamento dos Dados
O projeto segue um pipeline completo de preparação dos dados, incluindo:

- **Integração dos datasets** (`orders`, `order_items`, `products`)
- **Exploração inicial (EDA)**: análise de estrutura, tipos e distribuição
- **Limpeza de dados**:
  - remoção de inconsistências
  - tratamento de valores ausentes
  - identificação e ajuste de outliers via IQR
- **Conversão e padronização de tipos** (datas, numéricos e categóricos)
- **Tratamento de textos e categorias**
- **Codificação de variáveis categóricas** (One-Hot Encoding)
- **Normalização e padronização** (Min-Max e Z-score)
- **Seleção de atributos** com base em correlação e variância
- **Feature Engineering**, criando atributos como:
  - tempo_envio  
  - tempo_entrega_real  
  - preco_total  
  - percentual_frete  
  - dias_atraso  
- **Geração do dataset final** pronto para análise e modelagem

---

## ⚠️ Principais Desafios Encontrados
- Valores inconsistentes em datas que geravam tempos de entrega negativos  
- Outliers extremos em frete, preço e dimensões dos produtos  
- Categorias de produtos duplicadas ou mal formatadas  
- Diferenças de escala entre variáveis numéricas  
- Integração de múltiplos datasets mantendo consistência entre chaves  
- Necessidade de criar atributos que representassem melhor o fluxo logístico  

---

## 📘 Principais Conclusões
- O **tempo de envio do vendedor** foi o fator mais relevante para atrasos.  
- Categorias maiores e volumosas apresentaram mais problemas logísticos.  
- Outliers influenciavam significativamente as distribuições e precisavam de tratamento criterioso.  
- A engenharia de atributos permitiu entender melhor o comportamento da entrega e do frete.  
- O pré-processamento deixou os dados muito mais limpos, consistentes e adequados para análises posteriores.  

---

## 📎 Arquivos do Repositório
- Notebook completo (`.ipynb`)
- Dataset final pré-processado (`dataset_final.csv`)
- Relatório em PDF (`relatorio.pdf`)
- Dados originais em `/data` (opcional)
