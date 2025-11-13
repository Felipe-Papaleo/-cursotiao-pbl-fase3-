NOME DO PROJETO

PBL 1 (FASE 3)

Nome do grupo

Omni

👨‍🎓 Integrantes

Felipe Papaleo


👩‍🏫 Professores
Tutor(a)

Nome do Tutor(a)

Coordenador(a)

Nome do Coordenador(a)

📜 Descrição



Este projeto tem como objetivo demonstrar o processo de conexão, criação e importação de uma base de dados para o Oracle Database utilizando a ferramenta Oracle SQL Developer, bem como o versionamento do banco de dados através do GitHub.
A documentação inclui cada etapa da importação de arquivos CSV, criação da tabela, ajustes de tipos de dados, execução de consultas e exportação final da tabela em formato .sql para controle de versão no repositório.


🔧 Como executar o código
Pré-requisitos

Oracle Database (versão utilizada no projeto)

Oracle SQL Developer

Git + GitHub

Java (necessário para executar o SQL Developer)



▶️ Passo a passo completo – Importação da base CSV no Oracle SQL Developer



1. Acessando as tabelas e iniciando a importação

No painel de conexões do Oracle SQL Developer:

Expanda sua conexão

Clique com botão direito em Tables (Tabelas)

Selecione Importar Dados…

<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/f2bae04b-d2ac-4359-89e2-851092a29e65" />






2. Selecionando o arquivo CSV

Configurações utilizadas:

Origem: Arquivo Local

Formato: CSV

Codificação: UTF-8

Pré-visualização exibida corretamente

<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/cd90643d-bbfd-4653-9c68-845d51c87027" />







3. Escolhendo o método de importação

Método: Inserir

Nome da Tabela: SENSORES_AGRO
<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/c22dbc79-f285-445e-9ee0-92321cab43e2" />






4. Selecionando todas as colunas

A ferramenta automaticamente reconhece todas as colunas do CSV.
Confirme e avance.
<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/5bcee177-f8c6-4935-acfa-050cbefdacef" />







5. Ajustando tipos de dados

Exemplo da coluna “Fertilizer Name”:

Tipo: VARCHAR2

Tamanho: 26
<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/86f3fedb-f0ae-4039-8e86-f055eb2f33e4" />






6. Concluindo a importação

O SQL Developer exibe a mensagem:

"Importar Dados. Tarefa bem-sucedida e importação com commit efetuado."
<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/d40ece32-4595-442a-bcfb-f84a697bb677" />






7. Validando os dados importados

Execute uma consulta para validar a tabela:

SELECT * FROM SENSORES_AGRO;

<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/460e002f-7381-449b-bddf-438bb3bbefa0" />







9. Exportando corretamente a tabela como arquivo .sql

Use o Assistente de Exportação (Database Export) clicando com o botão direito do mouse em cima da tabela desejada, selecione export:

Marque Exportar DDL

Marque Exportar Dados

Formato: insert

Salvar como: Arquivo único

<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/b34db169-c4d7-4525-9caf-5ca5ce6593e3" />






10. Selecionando a tabela para exportação

Escolha SENSORES_AGRO e finalize o assistente. Pronto arquiv gerado

sql/sensores_agro.sql
<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/c5575d47-57b9-4153-a025-cdab10818fec" />


<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/ecac13d5-34af-415d-9e20-e64cb1283e8b" />


<img width="1920" height="1001" alt="image" src="https://github.com/user-attachments/assets/9638a8e4-5071-4e8f-bdce-2ec417c563cc" />







🗃 Histórico de lançamentos
0.5.0 - 12/11/2025
