# **Instruções de laboratório**

# Preparar dados no Power BI Desktop

**O tempo estimado para concluir o laboratório é de 45 minutos.**

Neste laboratório, você inicia o desenvolvimento de uma solução Power BI Desktop para a empresa Adventure Works. Envolve conectar-se aos dados de origem, visualizar os dados e usar técnicas de visualização de dados para entender as características e a qualidade dos dados de origem.

Neste laboratório, você aprenderá a:

- Abra o Power BI Desktop
- Definir opções do Power BI Desktop
- Conectar-se aos dados de origem
- Visualizar dados de origem
- Use técnicas de visualização de dados para entender melhor os dados

## **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. **Preparar dados no Power BI Desktop**
2. Carregar dados no Power BI Desktop
3. Projetar um modelo de dados no Power BI
4. Criar cálculos DAX no Power BI Desktop, Parte 1
5. Criar cálculos DAX no Power BI Desktop, Parte 2
6. Projetar um relatório no Power BI Desktop, Parte 1
7. Projetar um relatório no Power BI Desktop, Parte 2
8. Analise dados com visuais de IA
9. Criar um painel do Power BI
10. Aplicar segurança em nível de linha

## **Exercício 1: Preparar Dados**

Neste exercício, você criará oito consultas do Power BI Desktop. Seis consultas originarão dados do SQL Server e duas de arquivos CSV.

### **Tarefa 1: Salve o arquivo do Power BI Desktop**

Nesta tarefa, você primeiro salvará o arquivo do Power BI Desktop.

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image1.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image1.png)

2. Para fechar a janela de introdução, no canto superior direito da janela, clique em **X** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image2.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image2.png)

3. Para salvar o arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
4. Selecione **Salvar** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image3.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image3.png)

5. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
6. Na caixa **Nome do arquivo** , insira **Análise de vendas** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image4.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image4.png)

7. Clique **em Salvar** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image5.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image5.png)

   Dica: Você também pode salvar o arquivo clicando no ícone **Salvar localizado no canto superior esquerdo.**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image6.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image6.png)

### **Tarefa 2: definir as opções do Power BI Desktop**

Nesta tarefa, você definirá as opções do Power BI Desktop.

1. No Power BI Desktop, clique na guia da faixa de opções **Arquivo** para abrir o modo de exibição de bastidores.
2. À esquerda, selecione **Opções e configurações** e, em seguida, selecione **Opções** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image7.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image7.png)

3. Na janela **Opções** , à esquerda, no grupo **Arquivo Atual** , selecione **Carregamento de Dados** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image8.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image8.png)

   As configurações de **Carregamento de Dados** para o arquivo atual permitem opções de configuração que determinam os comportamentos padrão durante a modelagem.

4. No grupo **Relacionamentos** , desmarque as duas opções que já estão marcadas.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image9.png)

   Embora ter essas duas opções habilitadas possa ser útil ao desenvolver um modelo de dados, você as desativou anteriormente para dar suporte à experiência de laboratório. Ao criar relacionamentos no laboratório **Carregar Dados no Power BI Desktop** , você aprenderá por que está adicionando cada um.

5. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image10.png)

6. Salve o arquivo do Power BI Desktop.

### **Tarefa 3: obter dados do SQL Server**

Nesta tarefa, você criará consultas baseadas em tabelas do SQL Server.

1. Na guia da faixa de opções **Home , de dentro do grupo Dados** , clique em **SQL Server** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image11.png)

2. Na janela Banco de **Dados SQL Server , na caixa Servidor** , insira **localhost** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image12.png)

   Neste laboratório, você se conectará ao banco de dados SQL Server usando **localhost** . Essa não é uma prática recomendada ao criar suas próprias soluções. É porque as fontes de dados do gateway não podem resolver **localhost** .

3. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image13.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image13.png)

4. Se as credenciais forem solicitadas, na janela Banco de **Dados do SQL Server** , selecione **Usar minhas credenciais atuais** . Em seguida, **conecte-se** .
5. Na janela **Navegador** , à esquerda, expanda o banco de dados **AdventureWorksDW2020** .

   O banco de dados **AdventureWorksDW2020** é baseado no banco de dados de exemplo **AdventureWorksDW2017 .** Ele foi modificado para apoiar os objetivos de aprendizagem dos laboratórios do curso.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image17.png)

6. Selecione—mas não verifique—a tabela **DimEmployee** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image18.png)

7. No painel direito, observe uma visualização dos dados da tabela.

   Os dados de visualização permitem determinar as colunas e uma amostra de linhas.

8. Para criar consultas, marque a caixa de seleção ao lado das seis tabelas a seguir:
   - DimFuncionário
   - DimFuncionárioVendasTerritório
   - DimProduto
   - DimReseller
   - DimSalesTerritório
   - FatoRevendedorVendas
9. Para aplicar transformações aos dados das tabelas selecionadas, clique em **Transformar Dados** .

   Você não transformará os dados neste laboratório. Os objetivos deste laboratório se concentram na exploração e criação de perfil dos dados na janela do **Editor do Power Query .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image19.png)

### **Tarefa 4: Visualizar consultas do SQL Server**

Nesta tarefa você visualizará os dados das consultas do SQL Server. Primeiro, você aprenderá informações relevantes sobre os dados. Você também usará as ferramentas de qualidade de coluna, distribuição de coluna e perfil de coluna para entender os dados e avaliar a qualidade dos dados.

1. Na janela do **Power Query Editor** , à esquerda, observe o painel **Consultas .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image20.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image20.png)

   O painel **Consultas** contém uma consulta para cada tabela que você verificou.

2. Selecione a primeira consulta— **DimEmployee** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image21.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image21.png)

   A tabela **DimEmployee** no banco de dados do SQL Server armazena uma linha para cada funcionário. Um subconjunto das linhas desta tabela representa os vendedores, que serão relevantes para o modelo que você desenvolverá.

3. No canto inferior esquerdo, na barra de status, observe as estatísticas da tabela — a tabela tem 33 colunas e 296 linhas.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image22.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image22.png)

4. No painel de visualização de dados, role horizontalmente para revisar todas as colunas.
5. Observe que as últimas cinco colunas contêm links **de Tabela** ou **Valor .**

   Essas cinco colunas representam relacionamentos com outras tabelas no banco de dados. Eles podem ser usados para unir tabelas. Você unirá tabelas no laboratório **Carregar Dados no Power BI Desktop .**

6. Para avaliar a qualidade da coluna, na guia **Exibir da faixa de opções, no grupo Visualização de dados** , verifique **Qualidade da coluna** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image23.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image23.png)

   O recurso de qualidade da coluna permite determinar facilmente a porcentagem de valores válidos, de erro ou vazios encontrados nas colunas.

7. Para a coluna **Posição** (sexta última coluna), observe que 94% das linhas estão vazias (nulo).

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image24.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image24.png)

8. Para avaliar a distribuição da coluna, na guia **Exibir** da faixa de opções, de dentro do grupo **Visualização de dados** , marque **Distribuição da coluna** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image25.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image25.png)

9. Revise a coluna **Posição** novamente e observe que há quatro valores distintos e um valor exclusivo.
10. Revise a distribuição da coluna para a coluna **EmployeeKey** (primeira) — há 296 valores distintos e 296 valores exclusivos.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image26.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image26.png)

    Quando as contagens distintas e exclusivas são iguais, significa que a coluna contém valores exclusivos. Ao modelar, é importante que algumas tabelas de modelo tenham colunas exclusivas. Essas colunas exclusivas podem ser usadas para criar relacionamentos um-para-muitos, que você fará no laboratório **Model Data in Power BI Desktop .**

11. No painel **Consultas , selecione a consulta DimEmployeeSalesTerritory** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image27.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image27.png)

    A tabela **DimEmployeeSalesTerritory** armazena uma linha para cada funcionário e as regiões do território de vendas que eles gerenciam. A tabela suporta relacionar muitas regiões a um único funcionário. Alguns funcionários gerenciam uma, duas ou possivelmente mais regiões. Ao modelar esses dados, você precisará definir um relacionamento muitos para muitos.

12. No painel **Consultas , selecione a consulta DimProduct** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image28.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image28.png)

    A tabela **DimProduct** contém uma linha por produto vendido pela empresa.

13. Role horizontalmente para revelar as últimas colunas.
14. Observe a coluna **DimProductSubcategory** .

    Ao adicionar transformações a essa consulta no laboratório **Carregar Dados no Power BI Desktop** , você usará a coluna **DimProductSubcategory** para unir tabelas.

15. No painel **Consultas , selecione a consulta DimReseller** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image29.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image29.png)

    A tabela **DimReseller** contém uma linha por revendedor. Os revendedores vendem, distribuem ou agregam valor aos produtos Adventure Works.

16. Para visualizar os valores da coluna, na guia **Exibir** da faixa de opções, de dentro do grupo **Visualização de dados** , marque **Perfil da coluna** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image30.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image30.png)

17. Selecione o cabeçalho da coluna **BusinessType .**
18. Observe o novo painel abaixo do painel de visualização de dados.
19. Revise as estatísticas da coluna e a distribuição de valores no painel de visualização de dados.
20. Observe o problema de qualidade de dados: há dois rótulos para warehouse ( **Warehouse** e o Warehouse com erros ortográficos **)** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image31.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image31.png)

21. Passe o cursor sobre a barra **Ware House** e observe que há cinco linhas com esse valor.

    Você aplicará uma transformação para renomear essas cinco linhas no laboratório **Carregar Dados no Power BI Desktop .**

22. No painel **Consultas , selecione a consulta DimSalesTerritory** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image32.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image32.png)

    A tabela **DimSalesTerritory** contém uma linha por região de vendas, incluindo **sede corporativa** (sede). As regiões são atribuídas a um país e os países são atribuídos a grupos. No laboratório **Model Data in Power BI Desktop** , você criará uma hierarquia para dar suporte à análise em nível de região, país ou grupo.

23. No painel **Consultas , selecione a consulta FactResellerSales** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image33.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image33.png)

    A tabela **FactResellerSales** contém uma linha por linha de pedido de venda — um pedido de venda contém um ou mais itens de linha.

24. Revise a qualidade da coluna para a coluna **TotalProductCost** e observe que 8% das linhas estão vazias.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image34.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image34.png)

    A falta de valores de coluna **TotalProductCost é um problema de qualidade de dados.** Para resolver o problema, no laboratório **Carregar Dados no Power BI Desktop** , você aplicará transformações para preencher os valores ausentes usando o custo padrão do produto, que é armazenado na tabela **DimProduct relacionada.**

### **Tarefa 5: obter dados de um arquivo CSV**

Nesta tarefa, você criará uma consulta com base em um arquivo CSV.

1. Para adicionar uma nova consulta, na janela **Power Query Editor** , na guia da faixa de opções **Home , de dentro do grupo New Query** , clique na seta para baixo **New Source** e selecione **Text/CSV** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image35.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image35.png)

2. Na janela **Abrir , navegue até a pasta D:\PL300\Resources** e selecione o arquivo **ResellerSalesTargets.csv** .
3. Clique **em Abrir** .
4. Na janela **ResellerSalesTargets.csv , revise os dados de visualização.**
5. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image36.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image36.png)

6. No painel **Consultas** , observe a adição da consulta **ResellerSalesTargets .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image37.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image37.png)

   O arquivo CSV **ResellerSalesTargets contém uma linha por vendedor, por ano.** Cada linha registra 12 metas de vendas mensais (expressas em milhares). Observe que o ano comercial da empresa Adventure Works começa em 1º de julho.

7. Observe que nenhuma coluna contém valores vazios.

   Quando não há uma meta de vendas mensal, um caractere de hífen é armazenado.

8. Revise os ícones no cabeçalho de cada coluna, à esquerda do nome da coluna.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image38.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image38.png)

   Os ícones representam o tipo de dados da coluna. **123** é um número inteiro e **ABC** é texto.

   Você aplicará muitas transformações para obter um resultado de formato diferente que consiste em apenas três colunas: **Date** , **EmployeeKey** e **TargetAmount** no laboratório **Load Data in Power BI Desktop** .

### **Tarefa 6: obtenha dados adicionais de um arquivo CSV**

Nesta tarefa, você criará uma consulta adicional com base em um arquivo CSV diferente.

1. Use as etapas da tarefa anterior para criar uma consulta com base no arquivo **D:\PL300\Resources\ColorFormats.csv** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image39.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image39.png)

   O arquivo CSV **ColorFormats contém uma linha por cor do produto.** Cada linha registra os códigos HEX para formatar as cores de fundo e fonte. Você integrará esses dados aos dados da consulta **DimProduct no laboratório Carregar dados no Power BI Desktop** .

### **Tarefa 7: Concluir**

Nesta tarefa, você concluirá o laboratório.

1. Na guia da faixa de opções **Exibir , de dentro do grupo Visualização de dados** , desmarque as três opções de visualização de dados que foram habilitadas anteriormente neste laboratório:

   - Qualidade da coluna
   - Distribuição de colunas
   - Perfil da coluna

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image40.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image40.png)

2. Para salvar o arquivo do Power BI Desktop, na janela **Editor do Power Query , na exibição Arquivo** backstage, selecione **Salvar** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image41.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image41.png)

3. Quando solicitado a aplicar as consultas, clique em **Aplicar mais tarde** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image42.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/01-prepare-data-with-power-query-in-power-bi-desktop_image42.png)

   A aplicação das consultas carregará seus dados no modelo de dados. Você não está pronto para fazer isso, pois há muitas transformações que devem ser aplicadas primeiro.

4. Se você pretende iniciar o próximo laboratório, deixe o Power BI Desktop aberto.

   Você aplicará várias transformações às consultas e, em seguida, aplicará as consultas para carregá-las no modelo de dados no laboratório **Carregar Dados no Power BI Desktop .**

# Parabéns!
