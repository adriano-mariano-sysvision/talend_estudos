# Talend Estudos - Processamento de Pedidos
Projeto de treino em Talend para simular um fluxo ETL de processamento de pedidos.
# Objetivo
Ler arquivos CSV de pedidos e clientes, realizar junção pelo id_cliente, calcular valor_total, validar registros, remover duplicidades, separar pedidos por faixa de valor e gerar arquivos de saída.
# Estrutura do repositório
- job/ -> job exportado do Talend
- entrada/ -> arquivos CSV de entrada
- saida/ -> arquivos gerados pelo processamento
- prints/ -> captura de tela do job executado
# Fluxo do job
tFileInputDelimited -> tMap -> tFilterRow -> tUniqRow -> tReplicate -> tFilterRow -> tFileOutputDelimited
