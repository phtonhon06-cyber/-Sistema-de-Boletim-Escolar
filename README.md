# -Sistema-de-Boletim-Escolar
Aplicação de console (terminal) desenvolvida em TypeScript para gerenciar notas e faltas de alunos, gerando um boletim individual em .txt e armazenando um resumo de todos os alunos em um arquivo .csv.

✨ Funcionalidades
Coleta de Dados Interativa: Solicita o nome, a série, o total de faltas e as notas do aluno de forma interativa no terminal.

Múltiplas Matérias: Coleta 8 notas para cada uma das seguintes matérias:

Matemática

Português

Geografia

História

Química

Cálculo de Média: Calcula a média final para cada matéria.

Validação de Aprovação: Verifica o status do aluno com base em:

Nota: Aprovado se a média for maior ou igual a 7.0.

Presença: Aprovado se a presença for maior ou igual a 75% (máximo de 50 faltas em um ano de 200 dias letivos).

Geração de Arquivos:

Cria um boletim detalhado (.txt) para cada aluno cadastrado.

Mantém um banco de dados simples (.csv) com o resumo de todos os alunos, que pode ser aberto em planilhas como Excel ou Google Sheets.

🚀 Tecnologias Utilizadas
Node.js: Ambiente de execução para o JavaScript/TypeScript.

TypeScript: Superset do JavaScript que adiciona tipagem estática.

readline-sync: Biblioteca para capturar a entrada do usuário de forma síncrona no console.

📋 Pré-requisitos
Antes de começar, você vai precisar ter as seguintes ferramentas instaladas em sua máquina:

Git

Node.js (versão 18 ou superior)

npm (geralmente já vem instalado com o Node.js)

⚙️ Instalação e Configuração
Siga os passos abaixo para configurar o projeto em sua máquina local:

Clone o repositório:

Bash

# Substitua pela URL do seu repositório
git clone https://github.com/seu-usuario/boletim-escolar.git
Navegue até a pasta do projeto:

Bash

cd boletim-escolar
Instale as dependências do projeto:
Este comando irá baixar e instalar todas as bibliotecas necessárias (como o readline-sync e o typescript).

Bash

npm install
▶️ Como Executar a Aplicação
Depois de instalar as dependências, siga os passos abaixo para rodar o sistema:

Compile o código TypeScript:
Este comando transforma seu código .ts (da pasta src) em código .js (na pasta dist), que o Node.js consegue entender.

Bash

npx tsc
Execute a aplicação:
Este comando inicia o programa. Ele começará a fazer as perguntas no terminal.

Bash

node dist/index.js
O programa continuará pedindo dados de novos alunos até que você responda "não" (n) para a pergunta "Deseja cadastrar outro aluno?".

📂 Arquivos Gerados
Após cadastrar um aluno, uma pasta chamada data será criada na raiz do projeto com os seguintes arquivos:

Nome_Do_Aluno_Serie.txt: Um boletim completo com o desempenho em cada matéria, status de aprovação e frequência.

alunos.csv: Um arquivo de planilha que adiciona uma nova linha para cada aluno cadastrado, servindo como um registro geral.

Exemplo de Boletim (.txt)
--- BOLETIM ESCOLAR ---

Aluno: Joao da Silva
Série: 9o Ano

--- DESEMPENHO NAS MATÉRIAS ---

Matéria: Matematica
Notas: [8, 7, 9, 8.5, 6, 7.5, 10, 8]
Média Final: 8.00
Status: Aprovado

... (outras matérias) ...

--- FREQUÊNCIA ---
Total de Faltas: 25
Limite de Faltas: 50
Porcentagem de Presença: 87.50%
Status de Presença: Aprovado

--- RESULTADO FINAL ---
Status Geral: APROVADO
Feito por   Pedro Henrique Tonhon RA: 2507542
            Matheus Babler Silva RA: 2506053
            Eduardo Padilha Escuer RA: 2500241
            Gustavo Facioni RA: 2506276
            Gabriel Canuto RA: 2505604
