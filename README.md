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

Victor Robinson: - https://github.com/programadorcarioca

<hr></hr>

Ferramentas Utilizadas:

• SQL Server
• MySQL WorkBench
• Excel
• GitHub

Diagrama relacional

 ![Screenshot](diagrama/importante.png)

<h2>Perguntas</h2>

🔹 Quais atores mais atuaram nos episódios de Game of Thrones?<br>
   Código utilizado no MySQL:<br>
   SELECT actor, episodes_appeared<br>
   FROM persons_V4<br> 
   WHERE Episodes_appeared > 50;<br>
   
   ![Screenshot](imagens/pergunta1.jpeg)
   

🔹 Quais os episódios tiveram as melhores avaliações?<br>
   Código utilizado no MySQL:<br>
   SELECT Episode, Rating<br> 
   FROM got_episodes_V4<br> 
   WHERE Rating > 9.5;<br>
   
   ![Screenshot](imagens/pergunta2.jpeg)

🔹 Quais os episódios mais votados?<br>
   Código utilizado no MySQL:<br>
   SELECT Episode, Votes<br> 
   FROM got_episodes_V4<br> 
   WHERE votes > 37000;<br>
   
   ![Screenshot](imagens/pergunta3.jpeg)

🔹 Quais os episódios tiveram as maiores durações?<br>
   Código utilizado no MySQL:<br>
   SELECT Episode, Duration<br> 
   FROM got_episodes_V4<br> 
   WHERE Duration > 60;<br>
   
   ![Screenshot](imagens/pergunta4.jpeg)

🔹 Quais regiões possuem mais casas?<br>
   Código utilizado no MySQL:<br>
   SELECT Region, COUNT(*)<br> 
   FROM houses_V1<br> 
   GROUP BY Region<br> 
   HAVING COUNT(*) > 1;<br>
   
   ![Screenshot](imagens/pergunta5.jpeg)
    
    
    RESULTADOS GERAIS:
                                                                
   ![Screenshot](imagens/Resultados.jpeg)
