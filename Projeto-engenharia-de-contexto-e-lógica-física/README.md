# 🔍 Projeto Multi-Algoritmos: Auditoria, Saúde e Lógica Física

![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=flat&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)

Este repositório contém uma coleção de algoritmos desenvolvidos para resolver problemas de decisão em contextos reais. O projeto explora desde a **Auditoria de Dados Financeiros** e **Triagem Clínica** até à **Engenharia de Contexto e Lógica Física**, focando-se na automação, segurança e tratamento de anomalias (*outliers*).

---

## 📊 1. Auditoria de Dados e Tratamento de Outliers
Módulo focado na integridade de relatórios financeiros e deteção de fraudes ou erros de lançamento.

### 🧠 Conceitos Aplicados
* **Deteção de Outliers:** Identificação de valores que divergem drasticamente da média (pontos fora da curva), prevenindo distorções em análises globais.
* **Normalização:** Ajuste dos dados para refletir a realidade operacional, removendo ruído estatístico.
* **Limite de Materialidade:** Definição técnica da tolerância de erro aceitável antes de comprometer a confiança do auditor.

### ⚙️ Regra de Negócio
O algoritmo calcula a média de vendas e, se um valor exceder em **5x a média**, o sistema entra em estado de **REVISÃO MANUAL**, permitindo ao auditor validar a legitimidade e atualizar dinamicamente o limite de segurança.

---

## 🏥 2. Sistema de Triagem Clínica
Baseado em protocolos de classificação de risco, este módulo utiliza lógica condicional para priorizar atendimentos médicos.

| Categoria | Critérios (Sinais Vitais / Sintomas) | Conduta |
| :--- | :--- | :--- |
| **Emergência** | Temp > 39°C, FC > 120, Falta de Ar ou Convulsão | Atendimento Imediato |
| **Urgência** | Temp >= 37.5°C, Vómitos ou Dores Fortes | Prioridade na Fila |
| **Comum** | Sinais estáveis e sintomas leves | Atendimento Padrão |

---

## 🏗️ 3. Engenharia de Contexto e Lógica Física
Um estudo avançado sobre a tradução do mundo físico para a lógica de programação, aplicado ao **Algoritmo do Microclima Local** e fluxos de decisão quotidiana.

* **Análise de Microclima:** Monitorização de variáveis como Temperatura (°C), Humidade (%) e IQA (Índice de Qualidade do Ar) em diferentes coordenadas geográficas.
* **Lógica de Resiliência:** Discussão sobre a necessidade de **Redundância (Plano B)**. Se um sensor falhar, o sistema deve acionar alertas para intervenção humana imediata.
* **Decomposição de Problemas:** Aplicação de lógica para resolver impasses físicos (ex: portas trancadas ou obstáculos no percurso) como variáveis críticas de um sistema.

---

## 🛒 4. Automação Comercial e Tipagem
Módulo focado nas boas práticas de desenvolvimento em Python:
* **Conversão de Tipos:** Importância do uso de `int()` e `float()` em funções de `input()` para evitar erros de concatenação de strings em cálculos financeiros.
* **Estruturas de Iteração:** Uso correto de `range(1, meses + 1)` para garantir que todos os períodos de faturamento sejam processados respeitando o índice exclusivo do Python.

---

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10
* **Ambiente:** Jupyter Notebook / Google Colab
* **Metodologia:** Lógica Booleana, Estatística Descritiva e Fluxogramas de Decisão.

---

## 🔧 Como Executar
1. Clone o repositório.
2. Abra os ficheiros `.ipynb` no Jupyter ou Google Colab.
3. Execute as células sequencialmente para testar os algoritmos interativos.

---
*Projeto desenvolvido para fins académicos, integrando lógica de programação e engenharia de contexto.*
