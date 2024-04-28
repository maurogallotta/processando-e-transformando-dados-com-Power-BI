Processando e Transformando Dados com Power BI
Desafio de Projeto - Processando e Transformando Dados com Power BI

Bussiness Report no GITHUB

Objetivo do Projeto:
Fazer o processamento dos dados de um arquivo .csv fornecido, transformá-los com Power BI para criar um relatório empresarial corregindo os poblemas dos dados.

Ferramentas Utilizadas
Azure, Power BI e MYSQL Workbanch 8.0

Criei uma instância na Azure para o MySQL - Dica: use uma conta organizacional do tipo (IE- Instituição de Ensino), para evitar conflitos.

Criei o banco de dados com as bases fornecidas do curso.

Integrei o Power BI com MySQL Azure - Dicas: instale o Visual Studio(VSCODE) 2019 ou se já tiver instalado vá em Windows Updade e verifique se há alguma atualização de versão Windows e componentes do Visual Studio 2019, baixe a versão do Conector 8.0.28 ou 8.0.32, pois são as versões mais compatíveis com Windows 10 e Power BI por último verifique se você inseriu as credenciais do Azure no Power BI corretamente para evitar erros desnecessários.

Fazer as mudanças necessarias para base de dados do curso.

Etapas de Transformação:
Renominei todoas as colunas das tabelas - Dica: faça isso clicando duas vezes no cabeçalho da coluna.

Modifiquei os valores de "Salary" da tabela azure_company employee para o tipo (Número decimal fixo).

Modifiquei os valores de "Hours" da tabela azure_company works_on para o tipo (Número inteiro).

Na coluna "Hours" havia uma inconsistencia de dados 0 que transformei - Dica: para fazer isso selecione a coluna "Hours" com um clique e vá para a guia Página Inicial, nas opções da guia, clique em Substituir Valores, insira em Valor a Ser Localizado 0 e em Substituir por um valor de sua preferência.

Separar colunas complexas só se for o caso, por exemplo, um endereço completo que tenha vários complementos.

Para mesclar consultas "employee" e "departament" para criar uma tabela "employee" com o nome dos departamentos associados aos colaboradores -Dica: não precisa criar uma nova tabela "employee", uma vez que ela já existe. Na própria tabela azure_company employee, adicionei uma coluna chamada "Departament name". Para fazer isso vá até a tabela "employee", na guia Adicionar Coluna, clique na opção Coluna de Exemplos, vai aparecer uma coluna em branco renomeie como "Departament name".

Repita o passo anterior para criar as colunas de "collaborators" que é a coluna que você vai incluir os valores de cada "Last Name" e "First Name", coluna de "Managers" e uma coluna chamada "Departament location", com os nomes dos respectivos departamentos e localizações. Não esqueçam de atualizar depois que fizerem cada modificação.

O penúltimo passo do documento eu desconcideraria, mas como pode ser relevante é melhor fazer - Dica: duplique a tabela de "employee" e faça um Renome para azure_company collaborators_managers na guia Página Inicial, clique na opção Agrupar por, na tela que irá aparecer deixe o tipo de agrupamento como Básico escolha a coluna que você quer agrupar dê um nome para ela, em Operação escolha Max e em Coluna, escolha a coluna que você quer agrupar e em seguida aperte em "Ok".

IMPORTATE 
Planeje antes de fazer

Em caso de dúvidas, recorra as pessoas que já concluíram o desafio, pesquise no site da Microsoft Power BI, artigos, tópicos e peça ajuda ao ChatGPT(caso tenha conhecimento).
