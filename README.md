<h1># Banco de dados - Game of Thrones.</h1>

📜Contexto do Projeto:

Há um problema e precisam da nossa ajuda para resolver!
O cliente acumulou alguns conjuntos de dados e eles não conseguem ter uma visão padronizada desses dados.

📜O que é para fazer?

Nesse projeto nossa squad deverá montar um dashboard com base no conjunto de dados escolhidos pela equipe (Game of Thrones), a fim de realizar uma apresentação com a exploração dos dados.

📜 Objetivos do projeto:

⇨ Criar um repositório compartilhado com a squad para que seja possível fazer o backup tanto do esquema do banco quanto das queries elaboradas.

⇨ Ideação/Brainstorm sobre perguntas que podem ser respondidas pelos dados: Análise o conjunto de dados selecionado para que as perguntas sejam pertinentes.

⇨ Estruturar o esquema do banco de dados: A partir da avaliação do conjunto de dados fornecidos, modelar as tabelas do banco. Note que não é necessário mapear todas as colunas de todas as tabelas. Mantenha sua implementação simples construindo um modelo que atende às perguntas elaboradas pelo grupo.

⇨ Realizar carga no banco: Com base no esquema desenhado e criado, subir os dados presentes nos arquivos para o banco de dados a fim de verificar o funcionamento da solução encontrada.

⇨ Criar visualizações dos dados com base nas perguntas elaboradas: aqui vocês podem usar planilhas (Excel / Google), Metabase, Tableau, Power Bi, etc.

⇨ Montar uma apresentação a partir das perguntas e análise exploratória feita em cima do conjunto de dados selecionado.

<hr></hr>

<h2>Nossa Equipe - Squad 1</h2>

Juan Sales: https://github.com/Juangsales

Luan Martins: https://github.com/luanmartins8

Patrick: https://github.com/pkdev95

Rafael Ferreira: https://github.com/Rafael-Ferreira-RJ

Victor Robinson: -

<hr></hr>

Ferramentas Utilizadas:

• SQL Server
• MySQL WorkBench
• Excel
• GitHub

<h2>Perguntas</h2>

🔹 Quais atores mais atuaram nos episódios de Game of Thrones?
   Código utilizado no MySQL:
   SELECT actor, episodes_appeared 
   FROM persons_V4 
   WHERE Episodes_appeared > 50;
   
   ![Screenshot](imagens/pergunta1.jpeg)
   

🔹 Quais os episódios tiveram as melhores avaliações?
   SELECT Episode, Rating 
   FROM got_episodes_V4 
   WHERE Rating > 9.5;

🔹 Quais os episódios mais votados?
   SELECT Episode, Votes 
   FROM got_episodes_V4 
   WHERE votes > 37000;

🔹 Quais os episódios tiveram as maiores durações?
   SELECT Episode, Duration 
   FROM got_episodes_V4 
   WHERE Duration > 60;

🔹 Quais regiões possuem mais casas?
   SELECT Region, COUNT(*) 
   FROM houses_V1 
   GROUP BY Region 
   HAVING COUNT(*) > 1;
