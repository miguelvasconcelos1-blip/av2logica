# ==============================================================================
# PROVA PRÁTICA AV1 - 3º BIMESTRE
# ARQUIVO: av1_saneamento_dados.py
# Nome do Aluno:
# Data:
# ==============================================================================

cadastros_brutos = [
    "  joao da silva;11988887777  ",
    "  maria sousa;21977776666  ",
    "  carlos edgardo oliveira;31966665555  ",
    "  ana paula lima;41955554444  "
]

print("==================================================")
print("     SISTEMA DE SANEAMENTO DE DADOS - AV1        ")
print("==================================================\n")

for i in range(len(cadastros_brutos)):

    cadastro = cadastros_brutos[i].strip()

    dados = cadastro.split(";")

    nome = dados[0].upper()
    telefone = dados[1].strip()

    ddd = telefone[0:2]

    print(f"Funcionário: {nome} | DDD: {ddd} | Telefone: {telefone}")

print("\n==================================================")
print("             PROCESSAMENTO CONCLUÍDO              ")
print("==================================================")
