# **Instruções de laboratório**

# Carregar dados no Power BI Desktop

**O tempo estimado para concluir o laboratório é de 45 minutos.**

Neste laboratório, você começará a aplicar transformações a cada uma das consultas criadas no laboratório anterior. Em seguida, você aplicará as consultas para carregar cada uma como uma tabela no modelo de dados.

Neste laboratório, você aprenderá a:

- Aplique várias transformações
- Aplicar consultas para carregá-las no modelo de dados

## **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. Preparar dados no Power BI Desktop
2. **Carregar dados no Power BI Desktop**
3. Projetar um modelo de dados no Power BI
4. Criar cálculos DAX no Power BI Desktop, Parte 1
5. Criar cálculos DAX no Power BI Desktop, Parte 2
6. Projetar um relatório no Power BI Desktop, Parte 1
7. Projetar um relatório no Power BI Desktop, Parte 2
8. Analise dados com visuais de IA
9. Criar um painel do Power BI
10. Aplicar segurança em nível de linha

## **Exercício 1: Carregar dados**

Neste exercício, você aplicará transformações a cada uma das consultas criadas no laboratório anterior.

### **Tarefa 1: comece**

Nesta tarefa, você configurará o ambiente para o laboratório.

_Importante: Se você continua no laboratório anterior (e concluiu esse laboratório com êxito), não conclua esta tarefa; em vez disso, continue a partir da próxima tarefa._

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image1.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image1.png)

2. Para fechar a janela de introdução, no canto superior esquerdo da janela, clique em **X** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image2.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image2.png)

3. Para abrir o arquivo inicial do Power BI Desktop, clique na guia da faixa de opções **Arquivo** para abrir o modo de exibição de bastidores.
4. Selecione **Abrir relatório** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image3.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image3.png)

5. Clique **em Procurar relatórios** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image4.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image4.png)

6. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\02-load-data-with-power-query-in-power-bi-desktop\Starter** .
7. Selecione o arquivo de **Análise de Vendas** .
8. Clique **em Abrir** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image5.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image5.png)

9. Feche todas as janelas informativas que possam ser abertas.
10. Observe a mensagem de aviso amarela abaixo da faixa de opções.

    _A mensagem alerta você para o fato de que as consultas não foram aplicadas para carregar como tabelas de modelo. Você aplicará as consultas posteriormente neste laboratório._

11. Para dispensar a mensagem de aviso, à direita da mensagem de aviso amarela, clique em **X** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image6.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image6.png)

12. Para criar uma cópia do arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
13. Selecione **Salvar como** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image7.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image7.png)

14. Se solicitado a aplicar as alterações, clique em **Aplicar mais tarde** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image8.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image8.png)

15. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
16. Clique **em Salvar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image9.png)

17. Para abrir a janela do **Power Query Editor , na guia Home** da faixa de opções, de dentro do grupo **Consultas** , clique no ícone **Transform Data .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image10.png)

### **Tarefa 2: configurar a consulta do vendedor**

Nesta tarefa, você configurará a consulta do **Vendedor .**

1. Na janela **Editor do Power Query** , no painel **Consultas , selecione a consulta DimEmployee** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image11.png)

2. Para renomear a consulta, no painel **Configurações da Consulta** (localizado à direita), na caixa **Nome** , substitua o texto por **Vendedor** e pressione **Enter** .

   _O nome da consulta determinará o nome da tabela modelo. Recomenda-se definir nomes concisos, mas amigáveis._

3. No painel **Consultas , verifique se o nome da consulta foi atualizado.**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image12.png)

   _Agora você filtrará as linhas de consulta para recuperar apenas os funcionários que são vendedores._

4. Para localizar uma coluna específica, na guia da faixa de opções **Home** , clique na seta para baixo **Gerenciar Colunas , clique na seta para baixo Escolher Colunas** e selecione **Ir para Coluna** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image13.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image13.png)

   _Dica: Essa técnica é útil quando uma consulta contém muitas colunas. Se não houver muitas colunas, você pode simplesmente rolar horizontalmente para localizar a coluna de interesse._

5. Na janela **Ir para Coluna** , para ordenar a lista pelo nome da coluna, clique no botão de classificação **AZ** e selecione **Nome** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image14.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image14.png)

6. Selecione a coluna **SalesPersonFlag** e clique em **OK** .
7. Para filtrar a consulta, no cabeçalho da coluna **SalesPersonFlag** , clique na seta para baixo e desmarque **FALSE** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image15.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image15.png)

8. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image16.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image16.png)

9. No painel **Configurações de Consulta , na lista Etapas Aplicadas** , observe a adição da etapa **Linhas Filtradas .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image17.png)

   _Cada transformação que você cria resulta em lógica de etapa adicional. É possível editar ou excluir etapas. Também é possível selecionar uma etapa para visualizar os resultados da consulta nesse estágio da transformação da consulta._

10. Para remover colunas, na guia da faixa de opções **Home , clique no grupo Gerenciar Colunas** , clique no ícone **Escolher Colunas .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image18.png)

11. Na janela **Escolher Colunas** , para desmarcar todas as colunas, desmarque o item **(Selecionar todas as colunas)** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image19.png)

12. Para incluir colunas, verifique as seis colunas a seguir:
    - EmployeeKey
    - EmployeeNationalIDAlternateKey
    - Primeiro nome
    - Sobrenome
    - Título
    - Endereço de email
13. Clique **em OK** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image20.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image20.png)

14. Na lista **Etapas Aplicadas** , observe a adição de outra etapa de consulta.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image21.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image21.png)

15. Para criar uma coluna de nome único, primeiro selecione o cabeçalho da coluna **FirstName .**
16. Enquanto pressiona a tecla **Ctrl** , selecione a coluna **LastName .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image22.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image22.png)

17. Clique com o botão direito do mouse em um dos cabeçalhos de coluna selecionados e, no menu de contexto, selecione **Mesclar colunas** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image23.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image23.png)

    _Muitas transformações comuns podem ser aplicadas clicando com o botão direito do mouse no cabeçalho da coluna e escolhendo-as no menu de contexto. Observe, no entanto, que mais transformações estão disponíveis na faixa de opções._

18. Na janela **Mesclar Colunas , na lista suspensa Separador** , selecione **Espaço** .
19. Na caixa **Nome da Nova Coluna** , substitua o texto por **Vendedor** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image24.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image24.png)

20. Clique **em OK** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image25.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image25.png)

21. Para renomear a coluna **EmployeeNationalIDAlternateKey** , clique duas vezes no cabeçalho da coluna **EmployeeNationalIDAlternateKey .**
22. Substitua o texto por **EmployeeID** e pressione **Enter** .

    _Importante: Quando instruído a renomear colunas, é importante renomeá-las exatamente como descrito._

23. Use as etapas anteriores para renomear a coluna **EmailAddress para UPN** .

    _UPN é um acrônimo para User Principal Name._

24. No canto inferior esquerdo, na barra de status, verifique se a consulta tem cinco colunas e 18 linhas.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image26.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image26.png)

    _Importante: é importante que você não prossiga se sua consulta não produzir o resultado correto — não será possível concluir laboratórios posteriores. Se as colunas ou linhas da consulta não corresponderem, consulte as etapas desta tarefa para corrigir quaisquer problemas._

### **Tarefa 3: configurar a consulta SalespersonRegion**

Nesta tarefa, você configurará a consulta **SalespersonRegion .**

1. No painel **Consultas , selecione a consulta DimEmployeeSalesTerritory** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image27.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image27.png)

2. No painel **Configurações de consulta , renomeie a consulta para SalespersonRegion** .
3. Para remover as duas últimas colunas, primeiro selecione o cabeçalho da coluna **DimEmployee .**
4. Enquanto pressiona a tecla **Ctrl** , selecione o cabeçalho da coluna **DimSalesTerritory .**
5. Clique com o botão direito do mouse em um dos cabeçalhos de coluna selecionados e, no menu de contexto, selecione **Remover colunas** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image28.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image28.png)

6. Na barra de status, verifique se a consulta tem duas colunas e 39 linhas.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image29.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image29.png)

### **Tarefa 4: configurar a consulta do produto**

Nesta tarefa, você configurará a consulta do **produto .**

_Importante: Quando instruções detalhadas já tiverem sido fornecidas, as etapas do laboratório agora fornecerão instruções mais concisas. Se precisar de instruções detalhadas, você pode consultar as etapas das tarefas anteriores._

1. Selecione a consulta **DimProduct** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image30.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image30.png)

2. Renomeie a consulta para **Product** .
3. Localize a coluna **FinishedGoodsFlag** e filtre a coluna para recuperar produtos que são produtos acabados (ou seja, TRUE).
4. Remova todas as colunas, exceto as seguintes:
   - Chave do produto
   - Nome do Produto em Inglês
   - Custo padrão
   - Cor
   - DimProductSubcategory
5. Observe que a coluna **DimProductSubcategory** representa uma tabela relacionada (contém links de **valor ).**
6. No cabeçalho da coluna **DimProductSubcategory** , à direita do nome da coluna, clique no botão expandir.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image31.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image31.png)

7. Para desmarcar todas as colunas, desmarque o item **(Selecionar todas as colunas)** .
8. Verifique as colunas **EnglishProductSubcategoryName** e **DimProductCategory** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image32.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image32.png)

   _Ao selecionar essas duas colunas, uma transformação será aplicada para unir à tabela **DimProductSubcategory** e incluir essas colunas. A coluna **DimProductCategory** é, na verdade, outra tabela relacionada na fonte de dados._

9. Desmarque a caixa de seleção **Usar nome de coluna original como prefixo** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image33.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image33.png)

   \*Os nomes das colunas de consulta devem sempre ser exclusivos. Se deixada marcada, esta caixa de seleção prefixaria cada coluna com o nome da coluna expandida (neste caso, **DimProductSubcategory** ). Como se sabe que os nomes das colunas selecionadas não colidem com os nomes das colunas na consulta do **produto , a opção é desmarcada.\***

10. Clique **em OK** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image34.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image34.png)

11. Observe que a transformação resultou na adição de duas colunas e que a coluna **DimProductSubcategory** foi removida.
12. Expanda a coluna **DimProductCategory** e, em seguida, introduza apenas a coluna **EnglishProductCategoryName .**
13. Renomeie as quatro colunas a seguir:
    - **PortugueseProductName** to **Product**
    - **Custo Padrão** para **Custo Padrão** (incluir um espaço)
    - **PortugueseProductSubcategoryName** to **Subcategory**
    - **PortugueseProductCategoryName** to **Category**
14. Na barra de status, verifique se a consulta tem seis colunas e 397 linhas.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image35.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image35.png)

### **Tarefa 5: configurar a consulta do revendedor**

Nesta tarefa você irá configurar a consulta do **Revendedor .**

1. Selecione a consulta **DimReseller** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image36.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image36.png)

2. Renomeie a consulta para **Revendedor** .
3. Remova todas as colunas, exceto as seguintes:
   - Chave do revendedor
   - Tipo de Negócio
   - Nome do revendedor
   - DimGeography
4. Expanda a coluna **DimGeography** para incluir apenas as três colunas a seguir:

   - Cidade
   - StateProvinceName
   - EnglishCountryRegionName

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image37.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image37.png)

5. No cabeçalho da coluna **Tipo de negócio** , clique na seta para baixo e, em seguida, revise os valores de coluna distintos e observe a ortografia incorreta do depósito.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image38.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image38.png)

6. Clique com o botão direito do mouse no cabeçalho da coluna **Tipo de negócio** e selecione **Substituir valores** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image39.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image39.png)

7. Na janela **Substituir Valores** , configure os seguintes valores:

   - Na caixa **Valor a ser** localizado, insira **Ware House**
   - Na caixa **Substituir por** , insira **Armazém**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image40.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image40.png)

8. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image41.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image41.png)

9. Renomeie as quatro colunas a seguir:
   - **BusinessType** para **Business Type** (incluir um espaço)
   - **Nome do Revendedor** para **Revendedor**
   - **StateProvinceName** para **State-Province**
   - **PortugueseCountryRegionName** to **Country-Region**
10. Na barra de status, verifique se a consulta tem seis colunas e 701 linhas.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image42.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image42.png)

### **Tarefa 6: configurar a consulta de região**

Nesta tarefa, você configurará a consulta de **região .**

1. Selecione a consulta **DimSalesTerritory** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image43.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image43.png)

2. Renomeie a consulta para **Region** .
3. Remova todas as colunas, exceto as seguintes:
   - Chave de território de vendas
   - VendasTerritórioRegião
   - VendasTerritórioPaís
   - Grupo de território de vendas
4. Renomeie as três colunas a seguir:
   - **VendasTerritório** de região para **região**
   - **VendasTerritórioPaís** a **País**
   - **VendasTerritórioGrupo** a **Grupo**
5. Na barra de status, verifique se a consulta tem quatro colunas e 10 linhas.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image45.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image45.png)

### **Tarefa 7: configurar a consulta de vendas**

Nesta tarefa você irá configurar a consulta de **Vendas .**

1. Selecione a consulta **FactResellerSales** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image46.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image46.png)

2. Renomeie a consulta para **Sales** .
3. Remova todas as colunas, exceto as seguintes:

   - Número do pedido de vendas
   - Data do pedido
   - Chave do produto
   - Chave do revendedor
   - EmployeeKey
   - Chave de território de vendas
   - Quantidade do pedido
   - Preço unitário
   - Custo Total do Produto
   - Total de vendas
   - DimProduto

   _Você pode se lembrar no laboratório **Preparar Dados no Power BI Desktop** que uma pequena porcentagem de linhas **FactResellerSales** tinha valores de **TotalProductCost** ausentes . A coluna **DimProduct** foi incluída para recuperar a coluna de custo padrão do produto para ajudar a corrigir os valores ausentes._

4. Expanda a coluna **DimProduct** , desmarque todas as colunas e inclua apenas a coluna **StandardCost .**
5. Para criar uma coluna personalizada, na guia **Adicionar Coluna , no grupo Geral** , clique em **Coluna Personalizada** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image47.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image47.png)

6. Na janela **Coluna Personalizada , na caixa Nome da Nova Coluna** , substitua o texto por **Custo** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image48.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image48.png)

7. Na caixa **Fórmula de coluna personalizada** , insira a seguinte expressão (após o símbolo de igual):

   `if [TotalProductCost] = null then [OrderQuantity] * [StandardCost] else [TotalProductCost]`

   Para sua conveniência, você pode copiar a expressão do arquivo **D:\PL300\Labs\02-load-data-with-power-query-in-power-bi-desktop\Assets\Snippets.txt** .

8. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image49.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image49.png)

_Essa expressão testa se o valor **TotalProductCost** está ausente. Se for, produz um valor multiplicando o valor **OrderQuantity** pelo valor **StandardCost** ; caso contrário, ele usa o valor **TotalProductCost** existente ._

1. Remova as duas colunas a seguir:
   - Custo Total do Produto
   - Custo padrão
2. Renomeie as três colunas a seguir:
   - **PedidoQuantidade** para **Quantidade**
   - **Preço unitário** para **preço unitário** (incluir um espaço)
   - **VendasValor** para **Vendas**
3. Para modificar o tipo de dados da coluna, no cabeçalho da coluna **Quantidade , à esquerda do nome da coluna, clique no ícone 1.2** e selecione **Número Inteiro** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image50.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image50.png)

   _Configurar o tipo de dados correto é importante. Quando a coluna contém um valor numérico, também é importante escolher o tipo correto se você espera realizar cálculos matemáticos._

4. Modifique os seguintes tipos de dados de três colunas para **Número Decimal Fixo** .

   - Preço unitário
   - Vendas
   - Custo

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image51.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image51.png)

   _O tipo de dados de número decimal fixo armazena valores com precisão total e, portanto, requer mais espaço de armazenamento que o número decimal. É importante usar o tipo de número decimal fixo para valores financeiros ou taxas (como taxas de câmbio)._

5. Na barra de status, verifique se a consulta tem 10 colunas e mais de 999 linhas.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image52.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image52.png)

   _No máximo 1.000 linhas serão carregadas como dados de visualização para cada consulta._

### **Tarefa 8: configurar a consulta de destinos**

Nesta tarefa, você configurará a consulta de **Destinos .**

1. Selecione a consulta **ResellerSalesTargets .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image53.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image53.png)

2. Renomeie a consulta para **Destinos** .
3. Para desdinamizar as colunas de 12 meses ( **M01** - **M12** ), primeiro selecione os cabeçalhos das colunas **Year** e **EmployeeID .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image54.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image54.png)

4. Clique com o botão direito do mouse em qualquer um dos cabeçalhos de coluna selecionados e, no menu de contexto, selecione **Unpivot Other Columns** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image55.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image55.png)

5. Observe que os nomes das colunas agora aparecem na coluna **Atributo** e os valores aparecem na coluna **Valor .**
6. Aplique um filtro à coluna **Valor** para remover valores de hífen (-).

   _Você deve se lembrar de que o caractere de hífen foi usado no arquivo CSV de origem para representar zero (0)._

7. Renomeie as duas colunas a seguir:

   - **Atributo** para **MonthNumber** (não há espaço entre as duas palavras - ele será removido mais tarde)
   - **Valor** para **Alvo**

   _Agora você aplicará transformações para produzir uma coluna de data. A data será derivada das colunas **Year** e **MonthNumber** . Você criará a coluna usando o recurso **Colunas de Exemplos** ._

8. Para preparar os valores da coluna **MonthNumber** , clique com o botão direito do mouse no cabeçalho da coluna **MonthNumber** e selecione **Replace Values** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image56.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image56.png)

9. Na janela **Substituir valores , na caixa Valor a** ser localizado , insira **M** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image57.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image57.png)

10. Clique **em OK** .
11. Modifique o tipo de dados da coluna **MonthNumber para Whole Number** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image58.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image58.png)

12. Na guia **Adicionar Coluna , no grupo Geral** , clique no ícone **Coluna de Exemplos .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image59.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image59.png)

13. Observe que a primeira linha é para o ano **2017** e o mês número **7** .
14. Na coluna **Column1** , na primeira célula da grade, comece a inserir **07/01/2017** e pressione **Enter** .

    _A máquina virtual usa configurações regionais dos EUA, portanto, essa data é, na verdade, 1º de julho de 2017._

15. Observe que as células da grade são atualizadas com valores previstos.

    _O recurso previu com precisão que você está combinando valores das colunas **Year** e **MonthNumber** ._

16. Observe também a fórmula apresentada acima da grade de consulta.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image60.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image60.png)

17. Para renomear a nova coluna, clique duas vezes no cabeçalho da coluna **Mesclada .**
18. Renomeie a coluna como **TargetMonth** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image61.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image61.png)

19. Para adicionar a nova coluna, clique em **OK** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image62.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image62.png)

20. Remova as seguintes colunas:
    - Ano
    - Número do mês
21. Modifique os seguintes tipos de dados de coluna:
    - **Destino** como número decimal fixo
    - **TargetMonth** como data
22. Para multiplicar os valores de **Destino** por 1000, selecione o cabeçalho da coluna **Destino e, em seguida, na guia Transformar** da faixa de opções, de dentro do grupo **Coluna de número** , clique em **Padrão** e selecione **Multiplicar** .

    _Você pode lembrar que os valores alvo foram armazenados como milhares._

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image63.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image63.png)

23. Na janela **Multiplicar , na caixa Valor** , insira **1000** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image64.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image64.png)

24. Clique **em OK** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image65.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image65.png)

25. Na barra de status, verifique se a consulta tem três colunas e 809 linhas.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image66.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image66.png)

### **Tarefa 9: Configurar a consulta ColorFormats**

Nesta tarefa você irá configurar a consulta **ColorFormats** .

1. Selecione a consulta **ColorFormats** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image67.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image67.png)

2. Observe que a primeira linha contém os nomes das colunas.
3. Na guia da faixa de opções **Home , de dentro do grupo Transform** , clique em **Use First Row as Headers** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image68.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image68.png)

4. Na barra de status, verifique se a consulta tem três colunas e 10 linhas.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image69.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image69.png)

### **Tarefa 10: atualize a consulta do produto**

Nesta tarefa, você atualizará a consulta **Product** mesclando a consulta **ColorFormats** .

1. Selecione a consulta do **produto .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image70.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image70.png)

2. Para mesclar a consulta **ColorFormats** , na guia da faixa de opções **Home** , clique na seta para baixo **Combinar e clique em Mesclar consultas** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image71.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image71.png)

   _A mesclagem de consultas permite a integração de dados, neste caso de diferentes fontes de dados (SQL Server e um arquivo CSV)._

3. Na janela **Mesclar** , na grade de consulta **Produto** , selecione o cabeçalho da coluna **Cor .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image72.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image72.png)

4. Abaixo da grade de consulta do **produto** , na lista suspensa, selecione a consulta **ColorFormats** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image73.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image73.png)

5. Na grade de consulta **ColorFormats** , selecione o cabeçalho da coluna **Color .**
6. Quando a janela **Níveis de Privacidade** for aberta, para cada uma das duas fontes de dados, na lista suspensa correspondente, selecione **Organizacional** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image74.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image74.png)

   _Os níveis de privacidade podem ser configurados para a fonte de dados para determinar se os dados podem ser compartilhados entre as fontes. Definir cada fonte de dados como **Organizacional** permite que eles compartilhem dados, se necessário. Observe que as fontes de dados privadas nunca podem ser compartilhadas com outras fontes de dados. Isso não significa que os dados privados não possam ser compartilhados; significa que o mecanismo do Power Query não pode compartilhar dados entre as fontes._

7. Clique **em Salvar** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image75.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image75.png)

8. Na janela **Merge , use o Join Kind** padrão - mantendo a seleção de Left Outer e clique em **OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image76.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image76.png)

9. Expanda a coluna **ColorFormats** para incluir as duas colunas a seguir:

   - Formato de cor de fundo
   - Formato de cor da fonte

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image77.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image77.png)

10. Na barra de status, verifique se a consulta agora tem oito colunas e 397 linhas.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image78.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image78.png)

### **Tarefa 11: Atualize a consulta ColorFormats**

Nesta tarefa você atualizará os **ColorFormats** para desabilitar sua carga.

1. Selecione a consulta **ColorFormats** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image79.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image79.png)

2. No painel **Configurações de consulta** , clique no link **Todas as propriedades .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image80.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image80.png)

3. Na janela **Propriedades da consulta , desmarque a caixa de seleção Ativar carregamento para relatório** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image81.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image81.png)

   Desabilitar o carregamento significa que ele não será carregado como uma tabela para o modelo de dados. Isso é feito porque a consulta foi mesclada com a consulta do **produto** , que está habilitada para carregar no modelo de dados.

4. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image82.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image82.png)

### **Tarefa 12: Concluir**

Nesta tarefa, você concluirá o laboratório.

1. Verifique se você tem oito consultas, nomeadas corretamente da seguinte maneira:
   - Vendedor
   - Região do vendedor
   - produtos
   - Revendedor
   - Região
   - Vendas
   - Alvos
   - ColorFormats (que não será carregado no modelo de dados)
2. Para carregar o modelo de dados, na exibição **Arquivo** backstage, selecione **Fechar e Aplicar** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image83.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image83.png)

   _Todas as consultas habilitadas para carregamento agora são carregadas no modelo de dados._

3. No painel **Campos** (localizado à direita), observe as sete tabelas carregadas no modelo de dados.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image84.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/02-load-data-with-power-query-in-power-bi-desktop_image84.png)

4. Salve o arquivo do Power BI Desktop.
5. Se você pretende iniciar o próximo laboratório, deixe o Power BI Desktop aberto.

   \*Você configurará as tabelas e relacionamentos do modelo de dados no laboratório **Dados do Modelo no Power BI Desktop .\***

# **Parabéns!**
