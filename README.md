# Analise_de_Dados_com_o_Pandas
 Análise de Dados com o Pandas + Integração Python e Excel

Mini Projeto de Análise de Dados

Introdução

Este mini projeto tem como objetivo aplicar e reforçar os conhecimentos em Pandas e outros módulos de manipulação de dados no Python. Durante o projeto, trabalharemos com um conjunto de dados reais de uma empresa de prestação de serviços e responderemos perguntas importantes sobre os dados.

📂 Dados Disponíveis

Os arquivos utilizados neste projeto contêm informações da empresa no ano de 2019. Eles estão em formato CSV e XLSX:

CadastroFuncionarios.csv: Contém informações sobre os funcionários, incluindo salários e benefícios.

CadastroClientes.csv: Lista os clientes da empresa.

BaseServicosPrestados.xlsx: Registra os serviços realizados pela empresa.

📝 Como Ler os Arquivos no Pandas

Para arquivos CSV, usamos pd.read_csv().

Para arquivos XLSX (Excel), usamos pd.read_excel().

📊 Objetivos do Projeto

A partir dos dados fornecidos, responderemos as seguintes perguntas:

1️⃣ Valor Total da Folha Salarial

Pergunta: Qual foi o gasto total da empresa com salários em 2019?

Sugestão de Cálculo:

Calcular o salário total de cada funcionário: Salário Base + Benefícios + Impostos.

Somar os valores de todos os funcionários para obter o total.

2️⃣ Faturamento da Empresa

Pergunta: Qual foi o faturamento total da empresa?

Sugestão de Cálculo:

Calcular o faturamento de cada serviço (preço cobrado).

Somar o faturamento de todos os serviços.

3️⃣ Percentual de Funcionários que Fecharam Contratos

Pergunta: Qual o percentual de funcionários que participaram da venda de contratos?

Sugestão de Cálculo:

Identificar os funcionários que já fecharam algum serviço (usando a BaseServicosPrestados).

Contar os funcionários dessa lista, garantindo que cada um seja contado apenas uma vez.

Calcular:Qtde_Funcionarios_Fecharam_Serviço / Qtde_Funcionários_Totais

💡 Dica: O método .unique() pode ser usado para excluir valores duplicados em uma coluna:

funcionarios_unicos = dataframe['coluna_funcionario'].unique()

4️⃣ Total de Contratos Fechados por Área

Pergunta: Quantos contratos foram fechados por cada setor da empresa?

Sugestão de Cálculo:

Agrupar os serviços realizados por área e contar o total de contratos.

5️⃣ Total de Funcionários por Área

Pergunta: Quantos funcionários trabalham em cada setor da empresa?

Sugestão de Cálculo:

Contar a quantidade de funcionários em cada setor da empresa.

6️⃣ Ticket Médio Mensal dos Contratos

Pergunta: Qual o faturamento médio mensal da empresa?

Sugestão de Cálculo:

Calcular a média do faturamento mensal:

faturamento_mensal_medio = dataframe['faturamento'].mean()

🛠 Configurações de Encoding

Para evitar erros ao carregar os arquivos, utilize os seguintes encodings:
encoding='latin1'
encoding='ISO-8859-1'
encoding='utf-8'
encoding='cp1252'

Caso os arquivos CadastroClientes.csv e CadastroFuncionarios.csv apresentem erro ao importar, use o separador ";" (ponto e vírgula):
pd.read_csv('CadastroClientes.csv', sep=';')

🎯 Conclusão

Este projeto ajuda a consolidar os conhecimentos em Pandas, manipulação de dados, operações matemáticas e análise exploratória. Ao final, teremos um panorama completo do desempenho da empresa em 2019.


