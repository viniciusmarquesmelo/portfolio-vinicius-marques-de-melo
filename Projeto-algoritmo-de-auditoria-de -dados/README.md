# 🔍 Algoritmo de Auditoria de Dados

![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/status-conclu%C3%ADdo-brightgreen.svg)

## 📝 Descrição do Projeto
Este projeto consiste em um sistema experimental de auditoria de dados de vendas, focado na identificação de discrepâncias e na aplicação de conceitos fundamentais de análise estatística. O objetivo é automatizar a detecção de transações que fogem ao padrão (outliers) e estabelecer fluxos de revisão manual para garantir a integridade dos relatórios financeiros.

O trabalho explora a relação entre médias aritméticas, normalização de dados e níveis de materialidade em auditoria.

## 🧠 Conceitos Aplicados
O projeto aborda três pilares fundamentais da análise de dados:

1.  **Tratamento de Outliers:** Identificação de valores que distorcem a média geral de um conjunto de dados por estarem muito distantes do padrão estabelecido.
2.  **Normalização:** O processo de ajustar os dados (removendo ou tratando outliers) para obter um resultado fiel da realidade, evitando que valores extremos mascarem a performance real.
3.  **Limite de Materialidade:** Definição do valor máximo de erro ou distorção que um auditor pode aceitar sem comprometer a confiança das conclusões do relatório.

## 🚀 Funcionalidades
* **Entrada Dinâmica:** Coleta de dados de vendas via input do usuário.
* **Cálculo de Média:** Processamento automático da média das transações.
* **Detecção de Anomalias:** O sistema identifica automaticamente vendas que excedem em 5x a média calculada.
* **Fluxo de Revisão:** Interface de decisão para o auditor validar se transações discrepantes são legítimas ou necessitam de ajuste no limite de segurança.

## 🛠️ Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Ambiente:** Google Colab / Jupyter Notebook

## 📊 Análise de Riscos e Segurança
O projeto discute as implicações de sistemas de auditoria frágeis, destacando riscos como:
* Inconsistências de dados e falta de rastreabilidade.
* Vulnerabilidade a fraudes por falta de validação rigorosa.
* Distorção de resultados financeiros devido à influência de outliers não tratados.

## 🔧 Como Executar
1. Abra o arquivo `.ipynb` no **Google Colab** ou em um ambiente **Jupyter** local.
2. Execute as células de código.
3. Insira os valores de venda solicitados para testar o algoritmo de análise.

---
*Este projeto foi desenvolvido como parte de estudos práticos em Auditoria e Algoritmos.*
