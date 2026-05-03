# 🔍 Projeto Multi-Algoritmos: Auditoria, Saúde e Engenharia de Contexto

![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=flat&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)

Este repositório reúne uma série de algoritmos desenvolvidos para solucionar problemas reais através da lógica de programação. O projeto explora a automação de decisões, o tratamento de anomalias estatísticas e a tradução do mundo físico para fluxos lógicos computacionais.

---

## 📊 1. Auditoria de Dados e Tratamento de Outliers
Módulo focado na integridade de relatórios financeiros e na detecção de anomalias em transações de vendas.

### 🧠 Conceitos Estatísticos Aplicados
* **Deteção de Outliers:** Identificação de valores que divergem drasticamente do padrão (pontos fora da curva), evitando que um único valor alto mascare a realidade dos dados.
* **Normalização:** Processo de refinar o conjunto de dados para obter uma média fiel, eliminando distorções que fariam os dados parecerem maiores ou menores do que realmente são.
* **Materialidade:** Definição do valor máximo de erro ou distorção que um auditor aceita sem comprometer a confiança do relatório final.

### ⚙️ Lógica de Revisão
O sistema aplica uma regra de validação: se uma venda exceder em **5x a média**, o algoritmo dispara um alerta de **REVISÃO MANUAL**. Se confirmada a legitimidade pelo auditor, o limite de segurança é atualizado dinamicamente.

---

## 🏥 2. Sistema de Triagem Clínica (Protocolo de Risco)
Algoritmo de apoio à decisão hospitalar que utiliza sinais vitais para priorizar atendimentos.

| Nível de Risco | Critérios (Sinais Vitais/Sintomas) | Conduta |
| :--- | :--- | :--- |
| **Emergência** | Temp > 39°C, FC > 120, Falta de ar ou Convulsão | Atendimento Imediato |
| **Urgência** | Temp >= 37.5°C, Vómitos ou Dores Fortes | Prioridade na Fila |
| **Comum** | Sinais estáveis e sintomas leves | Atendimento Padrão |

### 🛡️ Resiliência e Fallback
O projeto prevê a gestão de falhas técnicas. Caso um sensor falhe ou apresente dados implausíveis, o sistema aciona automaticamente um **Plano B (Fallback)**: um alerta de intervenção humana para garantir que o paciente não fique sem assistência.

---

## 🏗️ 3. Engenharia de Contexto e Lógica Física
Um estudo avançado sobre como variáveis físicas (temperatura, obstáculos, chaves) influenciam fluxos de navegação e conforto.

* **Análise de Microclima:** Monitorização de Temperatura, Humidade e IQA (Índice de Qualidade do Ar) em coordenadas específicas de São Paulo, gerando uma "Nota de Conforto Urbano" ponderada.
* **Simulador de Evacuação:** Algoritmo que gere o movimento de um agente num ambiente físico, lidando com variáveis críticas como "Portas Trancadas", "Fumaça" e "Consumo de Energia".
* **Aprendizado:** A lógica demonstra que o progresso nem sempre é linear; por vezes, o sistema deve retroceder para recolher itens necessários (como chaves) para avançar num objetivo posterior.

---

## 🛒 4. Automação Comercial e Tipagem
Demonstração de boas práticas de programação em fluxos de caixa e faturamento.

* **Gestão de Tipagem:** Uso de `float()` e `int()` para garantir que entradas de utilizador (strings por padrão) possam ser processadas em cálculos de troco e faturamento mensal.
* **Decomposição de Notas:** Algoritmo para calcular a quantidade mínima de cédulas físicas (100, 50, 20, 10, 5, 2, 1) necessárias para o troco de uma operação.

---

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10
* **Ambiente:** Jupyter Notebook / Google Colab
* **Metodologia:** Lógica Booleana, Estruturas de Iteração (`range`), e Condicionais Aninhadas.

---

## 🔧 Como Executar
1. Clone o repositório.
2. Abra os ficheiros `.ipynb` no Jupyter ou Google Colab.
3. Execute as células sequencialmente para interagir com os simuladores e ferramentas de auditoria.

---
*Projeto desenvolvido para fins académicos, integrando lógica de programação e engenharia de contexto.*
