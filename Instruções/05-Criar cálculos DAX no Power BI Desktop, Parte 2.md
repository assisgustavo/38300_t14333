# **Instruções de laboratório**

# Criar cálculos DAX no Power BI Desktop, Parte 2

**O tempo estimado para concluir o laboratório é de 45 minutos.**

Neste laboratório, você criará medidas com expressões DAX envolvendo manipulação de contexto de filtro.

Neste laboratório, você aprenderá a:

- Use a função CALCULATE() para manipular o contexto do filtro
- Usar funções de inteligência de tempo

### **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. Preparar dados no Power BI Desktop
2. Carregar dados no Power BI Desktop
3. Projetar um modelo de dados no Power BI
4. Criar cálculos DAX no Power BI Desktop, Parte 1
5. **Criar cálculos DAX no Power BI Desktop, Parte 2**
6. Projetar um relatório no Power BI Desktop, Parte 1
7. Projetar um relatório no Power BI Desktop, Parte 2
8. Analise dados com visuais de IA
9. Criar um painel do Power BI
10. Aplicar segurança em nível de linha

## **Exercício 1: Trabalhar com Contexto de Filtro**

Neste exercício, você criará medidas com expressões DAX envolvendo manipulação de contexto de filtro.

### **Tarefa 1: comece**

Nesta tarefa, você configurará o ambiente para o laboratório.

_Importante: Se você continua no laboratório anterior (e concluiu esse laboratório com êxito), não conclua esta tarefa; em vez disso, continue a partir da próxima tarefa._

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image1.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image1.png)

2. Para fechar a janela de introdução, no canto superior esquerdo da janela, clique em **X** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image2.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image2.png)

3. Para abrir o arquivo inicial do Power BI Desktop, clique na guia da faixa de opções **Arquivo** para abrir o modo de exibição de bastidores.
4. Selecione **Abrir relatório** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image3.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image3.png)

5. Clique **em Procurar relatórios** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image4.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image4.png)

6. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\05-create-dax-calculations-in-power-bi-desktop-advanced\Starter** .
7. Selecione o arquivo de **Análise de Vendas** .
8. Clique **em Abrir** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image5.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image5.png)

9. Feche todas as janelas informativas que possam ser abertas.
10. Para criar uma cópia do arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
11. Selecione **Salvar como** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image6.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image6.png)

12. Se solicitado a aplicar as alterações, clique em **Aplicar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image7.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image7.png)

13. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
14. Clique **em Salvar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image8.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image8.png)

### **Tarefa 2: crie um visual de matriz**

Nesta tarefa, você criará um visual de matriz para apoiar o teste de suas novas medidas.

1. No Power BI Desktop, na exibição Relatório, crie uma nova página de relatório.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image9.png)

2. Na **página 3** , adicione um visual de matriz.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image10.png)

3. Redimensione o visual da matriz para preencher a página inteira.
4. Para configurar os campos visuais da matriz, no painel **Campos , arraste a região | Hierarquia de regiões** e solte-a dentro do visual.

   _Os laboratórios usam uma notação abreviada para fazer referência a um campo ou hierarquia. Ficará assim: **Região | Regiões** . Neste exemplo, **Região** é o nome da tabela e **Regiões** é o nome da hierarquia._

5. Adicione também o campo **Vendas | Campo de vendas** .
6. Para expandir toda a hierarquia, no canto superior direito do visual da matriz, clique no ícone de seta dupla bifurcada duas vezes.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image11.png)

   _Você deve se lembrar de que a hierarquia de **Regiões** tem os níveis **Grupo** , **País** e **Região** ._

7. Para formatar o visual, no painel **Visualizações** , selecione o painel **Formatar** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image12.png)

8. Na caixa **Pesquisar** , insira **Passou** .
9. Defina a propriedade **Layout escalonado como Desativado** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image14.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image14.png)

10. Verifique se o visual da matriz agora tem quatro cabeçalhos de coluna.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image15.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image15.png)

    _Na Adventure Works, as regiões de vendas são organizadas em grupos, países e regiões. Todos os países – exceto os Estados Unidos – têm apenas uma região, que recebe o nome do país. Como os Estados Unidos são um território de vendas tão grande, estão divididos em cinco regiões de vendas._

    _Você criará várias medidas neste exercício e as testará adicionando-as ao visual da matriz._

### **Tarefa 3: manipular o contexto do filtro**

Nesta tarefa, você criará várias medidas com expressões DAX que usam a função CALCULATE() para manipular o contexto do filtro.

1. Adicione uma medida à tabela **Sales** , com base na seguinte expressão:

   _Para sua conveniência, todas as definições de DAX neste laboratório podem ser copiadas do arquivo **D:\PL300\Labs\05-create-dax-calculations-in-power-bi-desktop-advanced\Assets\Snippets.txt** ._

   **DAX**

   ```
   Sales All Region =

   CALCULATE(SUM(Sales[Sales]), REMOVEFILTERS(Region))
   ```

   _A função CALCULATE() é uma função poderosa usada para manipular o contexto do filtro. O primeiro argumento recebe uma expressão ou uma medida (uma medida é apenas uma expressão nomeada). Os argumentos subsequentes permitem modificar o contexto do filtro._

   _A função REMOVEFILTERS() remove os filtros ativos. Ele pode receber nenhum argumento ou uma tabela, uma coluna ou várias colunas como seu argumento._

   \*Nessa fórmula, a medida avalia a soma da coluna **Vendas** em um contexto de filtro modificado, que remove quaisquer filtros aplicados às colunas da tabela **Região .\***

2. Adicione a medida **Sales All Region** ao visual da matriz.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image16.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image16.png)

3. Observe que a medida **Sales All Region** calcula o total de vendas de todas as regiões para cada região, país (subtotal) e grupo (subtotal).

   _A nova medida ainda não produziu um resultado útil. Quando as vendas de um grupo, país ou região são divididas por esse valor, produzirá uma proporção útil conhecida como “porcentagem do total geral”._

4. No painel **Campos , certifique-se de que a medida Sales All Region** esteja selecionada (quando selecionada, terá um plano de fundo cinza escuro) e, na barra de fórmulas, substitua o nome e a fórmula da medida pela seguinte fórmula:

   _Dica: Para substituir a fórmula existente, primeiro copie o snippet. Em seguida, clique dentro da barra de fórmulas e pressione **Ctrl+A** para selecionar todo o texto. Em seguida, pressione **Ctrl+V** para colar o snippet para substituir o texto selecionado. Em seguida, pressione **Enter** ._

   **DAX**

   ```
   Sales % All Region =
   ‎DIVIDE(
   ‎ SUM(Sales[Sales]),
   ‎ CALCULATE(
   ‎ SUM(Sales[Sales]),
   ‎ REMOVEFILTERS(Region)
   ‎ )
   ‎)
   ```

   \*A medida foi renomeada para refletir com precisão a fórmula atualizada. A função DIVIDE() divide a medida **Sales** (não modificada pelo contexto de filtro) pela medida **Sales** em um contexto modificado, que remove todos os filtros aplicados à tabela **Region .\***

5. No visual de matriz, observe que a medida foi renomeada e que agora aparecem valores diferentes para cada grupo, país e região.
6. Formate a medida **Sales % All Region** como uma porcentagem com duas casas decimais.
7. No visual de matriz, revise os valores da medida **Sales % All Region .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image17.png)

8. Adicione outra medida à tabela **Sales** , com base na seguinte expressão e formate como uma porcentagem:

   **DAX**

   ```
   Sales % Country =
   ‎DIVIDE(
   ‎ SUM(Sales[Sales]),
   ‎ CALCULATE(
   ‎ SUM(Sales[Sales]),
   ‎ REMOVEFILTERS(Region[Region])
   ‎ )
   ‎)
   ```

9. Observe que a fórmula de medida **Sales % Country** difere ligeiramente da fórmula de medida **Sales % All Region** .

   _A diferença é que o denominador modifica o contexto do filtro removendo filtros na coluna Região da **tabela Região** , nem todas as colunas da tabela **Região** . Isso significa que todos os filtros aplicados às colunas de grupo ou país são preservados. Ele alcançará um resultado que representa as vendas como uma porcentagem do país._

10. Adicione a medida **Sales % Country** ao visual da matriz.
11. Observe que apenas as regiões dos Estados Unidos produzem um valor que não é 100%.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image18.png)

    _Você deve se lembrar de que apenas os Estados Unidos têm várias regiões. Todos os outros países compreendem uma única região, o que explica por que todos são 100%._

12. Para melhorar a legibilidade dessa medida no visual, substitua a medida **Sales % Country** por essa fórmula aprimorada.

    **DAX**

    ```
    Sales % Country =
    ‎IF(
    ‎ ISINSCOPE(Region[Region]),
    ‎ DIVIDE(
    ‎ SUM(Sales[Sales]),
    ‎ CALCULATE(
    ‎ SUM(Sales[Sales]),
    ‎ REMOVEFILTERS(Region[Region])
    ‎ )
    ‎ )
    ‎)
    ```

    _Embutida na função IF(), a função ISINSCOPE() é usada para testar se a coluna de região é o nível em uma hierarquia de níveis. Quando true, a função DIVIDE() é avaliada. A ausência de uma parte falsa significa que em branco é retornado quando a coluna de região não está no escopo._

13. Observe que a medida **Sales % Country** agora só retorna um valor quando uma região está no escopo.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image19.png)

14. Adicione outra medida à tabela **Sales** , com base na seguinte expressão e formate como uma porcentagem:

    **DAX**

    ```
    Sales % Group =
    ‎DIVIDE(
    ‎ SUM(Sales[Sales]),
    ‎ CALCULATE(
    ‎ SUM(Sales[Sales]),
    ‎ REMOVEFILTERS(
    ‎ Region[Region],
    ‎ Region[Country]
    ‎ )
    ‎ )
    ‎)
    ```

    _Para obter vendas como uma porcentagem do grupo, dois filtros podem ser aplicados para remover efetivamente os filtros em duas colunas._

15. Adicione a medida **Sales % Group** ao visual da matriz.
16. Para melhorar a legibilidade dessa medida no visual, substitua a medida **Sales % Group** por essa fórmula aprimorada.

    **DAX**

    ```
    Sales % Group =
    ‎IF(
    ‎ ISINSCOPE(Region[Region])
    ‎ || ISINSCOPE(Region[Country]),
    ‎ DIVIDE(
    ‎ SUM(Sales[Sales]),
    ‎ CALCULATE(
    ‎ SUM(Sales[Sales]),
    ‎ REMOVEFILTERS(
    ‎ Region[Region],
    ‎ Region[Country]
    ‎ )
    ‎ )
    ‎ )
    ‎)
    ```

17. Observe que a medida **Sales % Group** agora só retorna um valor quando uma região ou país está no escopo.
18. Na visualização do modelo, coloque as três novas medidas em uma pasta de exibição chamada **Ratios** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image20.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image20.png)

19. Salve o arquivo do Power BI Desktop.

    _As medidas adicionadas à tabela **Sales** modificaram o contexto do filtro para obter uma navegação hierárquica. Observe que o padrão para obter o cálculo de um subtotal requer a remoção de algumas colunas do contexto do filtro e, para chegar a um total geral, todas as colunas devem ser removidas._

## **Exercício 2: Trabalhar com Inteligência de Tempo**

Neste exercício, você criará uma medida de vendas no acumulado do ano (YTD) e uma medida de crescimento de vendas ano a ano (YoY).

### **Tarefa 1: crie uma medida YTD**

Nesta tarefa, você criará uma medida de vendas YTD.

1. Na visualização Relatório, na **Página 2** , observe o visual de matriz que exibe várias medidas com anos e meses agrupados nas linhas.
2. Adicione uma medida à tabela **Sales** , com base na seguinte expressão e formatada com zero casas decimais:

   **DAX**

   ```
   Sales YTD =
   ‎TOTALYTD(SUM(Sales[Sales]), 'Date'[Date], "6-30")
   ```

   \*A função TOTALYTD() avalia uma expressão — neste caso, a soma da coluna **Sales** — em uma determinada coluna de data. A coluna de data deve pertencer a uma tabela de datas marcada como uma tabela de datas, como foi feito no laboratório **Criar Cálculos DAX no Power BI Desktop, Parte 1 .\***

   _A função também pode receber um terceiro argumento opcional representando a última data de um ano. A ausência desta data significa que 31 de dezembro é a última data do ano. Para Adventure Works, junho no último mês do ano, então “6-30” é usado._

3. Adicione o campo **Sales** e a medida **Sales YTD** ao visual da matriz.
4. Observe o acúmulo de valores de vendas dentro do ano.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image21.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image21.png)

   _A função TOTALYTD() executa a manipulação do filtro, especificamente a manipulação do filtro de tempo. Por exemplo, para calcular as vendas no ano de setembro de 2017 (o terceiro mês do ano fiscal), todos os filtros na tabela **Data** são removidos e substituídos por um novo filtro de datas que começam no início do ano (1º de julho de 2017) e estendendo-se até a última data do período de datas em contexto (30 de setembro de 2017)._

   _Observe que muitas funções de inteligência de tempo estão disponíveis no DAX para dar suporte a manipulações comuns de filtro de tempo._

### **Tarefa 2: crie uma medida de crescimento anual**

Nesta tarefa, você criará uma medida de crescimento de vendas YoY.

1. Adicione uma medida adicional à tabela **Sales** , com base na seguinte expressão:

   **DAX**

   ```
   Sales YoY Growth =
   ‎VAR SalesPriorYear =
   ‎ CALCULATE(
   ‎ SUM(Sales[Sales]),
   ‎ PARALLELPERIOD(
   ‎ 'Date'[Date],
   ‎ -12,
   ‎ MONTH
   ‎ )
   ‎ )
   ‎RETURN
   ‎ SalesPriorYear
   ```

   _A fórmula da medida **Sales YoY Growth** declara uma variável. As variáveis podem ser úteis para simplificar a lógica da fórmula e mais eficientes quando uma expressão precisa ser avaliada várias vezes dentro da fórmula (o que será o caso da lógica de crescimento YoY). As variáveis são declaradas por um nome exclusivo e a expressão de medida deve ser emitida após a palavra-chave **RETURN** ._

   _A variável **SalesPriorYear** recebe uma expressão que calcula a soma da coluna **Sales** em um contexto modificado que usa a função PARALLELPERIOD() para retroceder 12 meses a partir de cada data no contexto do filtro._

2. Adicione a medida **Sales YoY Growth** ao visual da matriz.
3. Observe que a nova medida retorna BLANK para os primeiros 12 meses (porque não houve vendas registradas antes do ano fiscal de 2017).
4. Observe que o valor da medida **Sales YoY Growth para julho de 2018** é o valor de **vendas para julho de 2017** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image22.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image22.png)

   _Agora que a “parte difícil” da fórmula foi testada, você pode substituir a medida pela fórmula final que calcula o resultado do crescimento._

5. Para completar a medida, substitua a medida **Sales YoY Growth** por esta fórmula, formatando-a como uma porcentagem com duas casas decimais:

   **DAX**

   ```
   Sales YoY Growth =
   ‎VAR SalesPriorYear =
   ‎ CALCULATE(
   ‎ SUM(Sales[Sales]),
   ‎ PARALLELPERIOD(
   ‎ 'Date'[Date],
   ‎ -12,
   ‎ MONTH
   ‎ )
   ‎ )
   ‎RETURN
   ‎ DIVIDE(
   ‎ (SUM(Sales[Sales]) - SalesPriorYear),
   ‎ SalesPriorYear
   ‎ )
   ```

6. Na fórmula, na cláusula **RETURN** , observe que a variável é referenciada duas vezes.
7. Verifique se o crescimento anual para **julho de 2018** é **de 392,83%** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image23.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image23.png)

   _Isso significa que as vendas de julho de 2018 (US$ 2.411.559) representam uma melhoria de quase 400% (quase 4x) em relação às vendas alcançadas no mesmo período do ano anterior (US$ 489.328)._

8. Na visualização do modelo, coloque as duas novas medidas em uma pasta de exibição chamada **Time Intelligence** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image24.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image24.png)

### **Tarefa 3: Concluir**

Nesta tarefa, você concluirá o laboratório.

1. Para limpar a solução pronta para o desenvolvimento de relatórios, no canto inferior esquerdo, clique com o botão direito do mouse na guia **Página 2** e selecione **Excluir** página.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image25.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image25.png)

2. Quando solicitado a excluir a página, clique em **Excluir** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image26.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/06-create-dax-calculations-in-power-bi-desktop-advanced_image26.png)

3. Apague a **página 3** também.
4. Na página restante, para limpar a página, selecione o visual da tabela e pressione a tecla **Delete** .
5. Salve o arquivo do Power BI Desktop.
6. Se você pretende iniciar o próximo laboratório, deixe o Power BI Desktop aberto.

   \*Você criará um relatório com base no modelo de dados no laboratório Criar um **Relatório no Power BI Desktop, Parte 1 .\***

# Parabéns!
