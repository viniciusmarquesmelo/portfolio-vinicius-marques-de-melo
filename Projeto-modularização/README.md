# 🔍 Projeto de Algoritmos Aplicados: Auditoria, Saúde e Comércio

![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)

Este repositório reúne o desenvolvimento de algoritmos lógicos e fluxogramas aplicados a três áreas críticas: **Auditoria de Dados**, **Triagem Clínica** e **Sistemas de Automação Comercial**.

---

## 📊 1. Algoritmo de Auditoria de Dados (Python)
Módulo focado na identificação de anomalias financeiras e integridade de relatórios de vendas.

### 🧠 Conceitos Estatísticos Implementados
* **Outliers:** Identificação de valores que divergem drasticamente do padrão (ex: uma venda isolada de R$ 5.000,00 quando a média é R$ 200,00).
* **Normalização:** Processo de refinar os dados para obter uma média real, evitando que valores extremos mascarem a performance da maioria dos casos.
* **Limite de Materialidade:** Definição do valor máximo de distorção que um auditor aceita sem comprometer a confiança do relatório final.

### ⚙️ Lógica do Código
O sistema calcula a média de vendas e aplica uma regra de validação:
- Se uma venda exceder em **5x a média**, o sistema entra em estado de **REVISÃO MANUAL**.
- O auditor deve validar a legitimidade; se confirmada, o **Limite de Segurança** é atualizado automaticamente.

---

## 🏥 2. Sistema de Triagem Clínica
Fluxograma e lógica condicional para classificação de risco hospitalar com base em sinais vitais.

### 🌡️ Parâmetros de Decisão
| Categoria | Sintomas / Sinais Vitais | Encaminhamento |
| :--- | :--- | :--- |
| **Emergência** | Temp > 39°C, FC > 120, Falta de Ar ou Convulsão | Atendimento Imediato |
| **Urgência** | Temp >= 37.5°C, Vómitos ou Dores Fortes | Prioridade na Fila |
| **Comum** | Sintomas leves e sinais estáveis | Atendimento Padrão |

### 🛡️ Resiliência do Sistema
- **Validação de Dados:** Proteção contra erros de leitura ou sensores avariados.
- **Plano B (Fallback):** Caso um sensor falhe, o sistema aciona um alerta automático para intervenção humana, garantindo que o paciente nunca fique sem assistência por falha técnica.

---

## 🛒 3. Automação de Caixa e Troco
Lógica para registro de produtos, cálculo de total e decomposição de troco em notas físicas.

### 🧩 Estrutura de Módulos
* **Registro:** Loop interativo para entrada de nomes e preços de produtos.
* **Validação de Pagamento:** Verifica se o valor pago é suficiente para cobrir o total.
* **Decomposição de Troco:** Algoritmo que calcula a quantidade mínima de notas (R$ 100, 50, 20, 10, 5, 2 e 1) a serem entregues ao cliente.

---

## 🚀 Tecnologias e Ferramentas
* **Linguagem:** Python 3.10
* **Ambiente:** Jupyter Notebook / Google Colab
* **Documentação Lógica:** Fluxogramas manuais e pseudocódigo.

---

## 🔧 Como Utilizar
1.  Abra o ficheiro `Projeto-algoritmo-de-auditoria-de-dados.ipynb` no Jupyter ou Colab para testar o sistema de auditoria.
2.  Consulte os fluxogramas para entender a arquitetura de decisão do sistema de triagem e do sistema comercial.

---
*Este projeto foi desenvolvido como parte de um estudo prático sobre lógica de programação, segurança de dados e processos de automação.*
