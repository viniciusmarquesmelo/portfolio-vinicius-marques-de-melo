# 🛡️ Sistema de Auditoria de Recursos Corporativos

Este projeto é um sistema em Python que automatiza a verificação de orçamentos em estruturas empresariais complexas, utilizando conceitos de recursividade e decoradores para garantir uma auditoria precisa e performática.

## 🚀 Como o código foi organizado

A lógica da **recursão** foi o que mais me fez quebrar a cabeça, mas pensei nela como se estivesse abrindo pastas dentro de pastas no computador. A função `percorrer_dicionario` olha cada item: se ela encontra um valor (dinheiro), ela soma; se encontra um outro "pacote" (um dicionário), ela mergulha lá dentro e faz tudo de novo até não sobrar mais nada. É o famoso "dividir para conquistar"!

O **decorator** (`@auditor`) foi acoplado como uma "capa" ou um vigilante em volta da função principal. Em vez de sujar o código de cálculo com logs e cronômetros, eu usei o decorator para interceptar a execução. Ele anota o horário de início, vê quais argumentos eu passei (como os setores que ignorei no `*args`) e calcula o tempo total de processamento sozinho. Ficou bem modular e fácil de dar manutenção!

* **Dados:** Os dados simulados da empresa foram estruturados em um **dicionário aninhado (Tree Data Structure)**. A "Matriz" é o tronco principal, e dentro dela temos os departamentos como "TI" e "RH", que funcionam como galhos. Esses galhos podem ter valores diretos ou outros sub-departamentos (folhas), permitindo que o sistema navegue por toda a hierarquia da empresa de forma dinâmica.

## 💻 Código Fonte

```python
import time

# O Decorator (Vinícius Marques)
def auditor(funcao_original):
    def wrapper(*args, **kwargs):
        print("Iniciando a verificacao do orcamento")
        tempo_inicio = time.time()
        
        resultado = funcao_original(*args, **kwargs)
        
        tempo_fim = time.time()
        tempo_gasto = tempo_fim - tempo_inicio
        
        print("Argumentos usados:", args)
        print("Tempo total de processamento:", tempo_gasto)
        print("Finalizado com sucesso")
        return resultado
    return wrapper

@Viniciusmarquesmelo
def calcular_orcamento(*setores_para_pular, **configuracao_moeda):
    empresa = {
        "Matriz": {
            "TI": {
                "Infraestrutura": 10000,
                "Software": 20000
            },
            "RH": {
                "Recrutamento": 5000,
                "Folha": 15000
            },
            "Vendas": 30000
        }
    }

    def percorrer_dicionario(dados_atuais):
        soma = 0
        for nome, valor in dados_atuais.items():
            if nome in setores_para_pular:
                continue
            if isinstance(valor, dict):
                soma += percorrer_dicionario(valor)
            else:
                soma += valor
        return soma

    total_bruto = percorrer_dicionario(empresa)
    taxa = configuracao_moeda.get("taxa_cambio", 1)
    total_final = total_bruto * taxa

    print("Valor total calculado:", total_final)
    return total_final

if __name__ == "__main__":
    calcular_orcamento("RH", taxa_cambio=5.20)
