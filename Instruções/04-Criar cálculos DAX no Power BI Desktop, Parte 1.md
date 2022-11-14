# **Instruções de laboratório**

# Criar cálculos DAX no Power BI Desktop, Parte 1

**O tempo estimado para concluir o laboratório é de 45 minutos.**

Neste laboratório, você criará tabelas calculadas, colunas calculadas e medidas simples usando expressões de análise de dados (DAX).

Neste laboratório, você aprenderá a:

- Criar tabelas calculadas
- Criar colunas calculadas
- Criar medidas

### **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. Preparar dados no Power BI Desktop
2. Carregar dados no Power BI Desktop
3. Projetar um modelo de dados no Power BI
4. **Criar cálculos DAX no Power BI Desktop, Parte 1**
5. Criar cálculos DAX no Power BI Desktop, Parte 2
6. Projetar um relatório no Power BI Desktop, Parte 1
7. Projetar um relatório no Power BI Desktop, Parte 2
8. Analise dados com visuais de IA
9. Criar um painel do Power BI
10. Aplicar segurança em nível de linha

## **Exercício 1: Criar Tabelas Calculadas**

Neste exercício, você criará duas tabelas calculadas. A primeira será a tabela **Vendedor** , para permitir uma relação direta entre ela e a tabela **Vendas .** A segunda será a tabela **Data .**

### **Tarefa 1: comece**

Nesta tarefa, você configurará o ambiente para o laboratório.

_Importante: Se você continua no laboratório anterior (e concluiu esse laboratório com êxito), não conclua esta tarefa; em vez disso, continue a partir da próxima tarefa._

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image1.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image1.png)

2. Para fechar a janela de introdução, no canto superior esquerdo da janela, clique em **X** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image2.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image2.png)

3. Para abrir o arquivo inicial do Power BI Desktop, clique na guia da faixa de opções **Arquivo** para abrir o modo de exibição de bastidores.
4. Selecione **Abrir relatório** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image3.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image3.png)

5. Clique **em Procurar relatórios** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image4.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image4.png)

6. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\04-create-dax-calculations-in-power-bi-desktop\Starter** .
7. Selecione o arquivo de **Análise de Vendas** .
8. Clique **em Abrir** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image5.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image5.png)

9. Feche todas as janelas informativas que possam ser abertas.
10. Para criar uma cópia do arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
11. Selecione **Salvar como** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image6.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image6.png)

12. Se solicitado a aplicar as alterações, clique em **Aplicar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image7.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image7.png)

13. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
14. Clique **em Salvar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image8.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image8.png)

### **Tarefa 2: Crie a tabela Vendedor**

Nesta tarefa, você criará a tabela **Vendedor** (relação direta com **Vendas** ).

1. No Power BI Desktop, na exibição Relatório, na faixa de **opções Modelagem , de dentro do grupo Cálculos** , clique em **Nova Tabela** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image9.png)

2. Na barra de fórmulas (que se abre diretamente abaixo da faixa de opções ao criar ou editar cálculos), digite **Vendedor =** , pressione **Shift+Enter** , digite **'Vendedor (Desempenho)'** e pressione **Enter** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image10.png)

   _Para sua conveniência, todas as definições de DAX neste laboratório podem ser copiadas do arquivo de snippets, localizado em **D:\PL300\Labs\04-create-dax-calculations-in-power-bi-desktop\Assets\Snippets.txt** ._

   _Uma tabela calculada é criada inserindo primeiro o nome da tabela, seguido pelo símbolo de igual (=), seguido por uma fórmula DAX que retorna uma tabela. Observe que o nome da tabela ainda não pode existir no modelo de dados._

   _A barra de fórmulas suporta a inserção de uma fórmula DAX válida. Inclui recursos como preenchimento automático, Intellisense e codificação por cores, permitindo que você insira a fórmula com rapidez e precisão._

   _Essa definição de tabela cria uma cópia da tabela **Vendedor (Desempenho)** . Ele copia apenas os dados, mas as propriedades do modelo, como visibilidade, formatação, etc., não são copiadas._

   _Dica: Você é encorajado a inserir “espaços em branco” (ou seja, retornos de carro e tabulações) para as fórmulas de layout em um formato intuitivo e fácil de ler—especialmente quando as fórmulas são longas e complexas. Para inserir um retorno de carro, pressione **Shift+Enter** . “Espaço em branco” é opcional._

3. No painel **Campos** , observe que o ícone da tabela é um tom de azul (indicando uma tabela calculada).

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image11.png)

   _As tabelas calculadas são definidas usando uma fórmula DAX que retorna uma tabela. É importante entender que as tabelas calculadas aumentam o tamanho do modelo de dados porque se materializam e armazenam valores. Eles são recalculados sempre que as dependências de fórmula são atualizadas, como será o caso desse modelo de dados quando novos valores de data (futuros) forem carregados em tabelas._

   _Ao contrário das tabelas de origem do Power Query, as tabelas calculadas não podem ser usadas para carregar dados de fontes de dados externas. Eles só podem transformar dados com base no que já foi carregado no modelo de dados._

4. Alterne para a visualização Modelo.
5. Observe que a tabela **Salesperson** está disponível (cuidado, ela pode estar oculta, nesse caso role horizontalmente para localizá-la).
6. Criar um relacionamento do **Vendedor | coluna EmployeeKey** para a coluna **Sales |** Coluna **EmployeeKey .**
7. Clique com o botão direito do mouse no relacionamento inativo entre as tabelas **Vendedor (Desempenho)** e **Vendas** e selecione **Excluir** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image12.png)

8. Quando solicitado a confirmar a exclusão, clique em **OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image13.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image13.png)

9. Na tabela **Vendedor** , selecione as seguintes colunas e, em seguida, oculte-as (defina a propriedade **Is Hidden como Yes** ):
   - ID do Empregado
   - EmployeeKey
   - UPN
10. No diagrama de modelo, selecione a tabela **Vendedor .**
11. No painel **Propriedades , na caixa Descrição** , insira: **Vendedor relacionado a Vendas**

    _Você deve se lembrar de que as descrições aparecem como dicas de ferramentas no painel **Campos** quando o usuário passa o cursor sobre uma tabela ou campo._

12. Para a tabela **Vendedor (Desempenho)** , defina a descrição como: **Vendedor relacionado à(s) região(ões)**

    _O modelo de dados agora oferece duas alternativas ao analisar vendedores. A tabela **Vendedor** permite analisar as vendas realizadas por um vendedor, enquanto a tabela **Vendedor (Desempenho)** permite analisar as vendas realizadas na(s) região(ões) de vendas atribuídas ao vendedor._

### **Tarefa 3: Crie a tabela de datas**

Nesta tarefa você criará a tabela **Data .**

1. Mude para a visualização de dados.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image14.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image14.png)

2. Na guia da faixa de opções **Home , de dentro do grupo Cálculos** , clique em **Nova Tabela** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image15.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image15.png)

3. Na barra de fórmulas, digite o seguinte:

   **DAX**

   ```
   Date =
   CALENDARAUTO(6)
   ```

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image16.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image16.png)

   _A função CALENDARAUTO() retorna uma tabela de coluna única que consiste em valores de data. O comportamento “automático” verifica todas as colunas de data do modelo de dados para determinar os valores de data mais antigos e mais recentes armazenados no modelo de dados. Em seguida, ele cria uma linha para cada data dentro desse intervalo, estendendo o intervalo em qualquer direção para garantir que anos completos de dados sejam armazenados._

   _Essa função pode receber um único argumento opcional que é o último número do mês de um ano. Quando omitido, o valor é 12, significando que dezembro é o último mês do ano. Nesse caso, 6 é inserido, o que significa que junho é o último mês do ano._

4. Observe a coluna de valores de data.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image17.png)

   _As datas mostradas são formatadas usando as configurações regionais dos EUA (ou seja, mm/dd/aaaa)._

5. No canto inferior esquerdo, na barra de status, observe as estatísticas da tabela, confirmando que foram geradas 1826 linhas de dados, o que representa dados de cinco anos completos.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image18.png)

### **Tarefa 4: crie colunas calculadas**

Nesta tarefa, você adicionará colunas adicionais para permitir a filtragem e o agrupamento por diferentes períodos de tempo. Você também criará uma coluna calculada para controlar a ordem de classificação de outras colunas.

_Para sua conveniência, todas as definições de DAX neste laboratório podem ser copiadas do arquivo de snippets, localizado em **D:\PL300\Labs\04-create-dax-calculations-in-power-bi-desktop\Assets\Snippets.txt** ._

1. Na faixa contextual **Ferramentas de Tabela , no grupo Cálculos** , clique em **Nova Coluna** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image19.png)

2. Na barra de fórmulas, digite o seguinte (ou copie do arquivo de trechos) e pressione **Enter** :

   **DAX**

   ```
   Year =
   "FY" & YEAR('Date'[Date]) + IF(MONTH('Date'[Date]) > 6, 1)
   ```

   _Uma coluna calculada é criada inserindo primeiro o nome da coluna, seguido pelo símbolo de igual (=), seguido por uma fórmula DAX que retorna um resultado de valor único. O nome da coluna ainda não pode existir na tabela._

   _A fórmula usa o valor do ano da data, mas adiciona um ao valor do ano quando o mês é posterior a junho. É como os anos fiscais da Adventure Works são calculados._

3. Verifique se a nova coluna foi adicionada.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image20.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image20.png)

4. Use as definições de arquivo de snippets para criar as duas colunas calculadas a seguir para a tabela **Data :**

   - Trimestre
   - Mês

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image21.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image21.png)

5. Para validar os cálculos, alterne para a visualização Relatório.
6. Para criar uma nova página de relatório, no canto inferior esquerdo, clique no ícone de adição.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image22.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image22.png)

7. Para adicionar um visual de matriz à nova página de relatório, no painel **Visualizações** , selecione o tipo de visual de matriz.

   _Dica: você pode passar o cursor sobre cada ícone para revelar uma dica de ferramenta descrevendo o tipo visual._

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image23.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image23.png)

8. No painel **Campos** , de dentro da tabela **Data** , arraste o campo **Ano** para o poço/área **Linhas .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image24.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image24.png)

9. Arraste o campo **Mês para o poço/área Linhas** , diretamente abaixo do campo **Ano** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image25.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image25.png)

10. No canto superior direito do visual da matriz (ou inferior, dependendo da localização do visual), clique no ícone de seta dupla bifurcada (que expandirá todos os anos um nível abaixo).

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image26.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image26.png)

11. Observe que os anos se expandem para meses e que os meses são classificados em ordem alfabética e não cronológica.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image27.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image27.png)

    _Por padrão, os valores de texto são classificados em ordem alfabética, os números são classificados do menor para o maior e as datas são classificadas do mais antigo para o mais recente._

12. Para personalizar a ordem de classificação do campo **Mês** , alterne para a exibição Dados.
13. Adicione a coluna **MonthKey** à tabela **Date .**

    **DAX**

    ```
    MonthKey =
    (YEAR('Date'[Date]) * 100) + MONTH('Date'[Date])
    ```

    _Esta fórmula calcula um valor numérico para cada combinação de ano/mês._

14. Na exibição de dados, verifique se a nova coluna contém valores numéricos (por exemplo, 201707 para julho de 2017 etc.).

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image28.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image28.png)

15. Volte para a visualização Relatório.
16. No painel **Campos , certifique-se de que o campo Mês** esteja selecionado (quando selecionado, terá um fundo cinza escuro).
17. Na faixa contextual **Ferramentas de Coluna , no grupo Classificar** , clique em **Classificar por Coluna** e selecione **MonthKey** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image29.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image29.png)

18. No visual de matriz, observe que os meses agora estão ordenados cronologicamente.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image30.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image30.png)

### **Tarefa 5: Preencha a tabela de datas**

Nesta tarefa, você concluirá o design da tabela **Data** ocultando uma coluna e criando uma hierarquia. Em seguida, você criará relacionamentos com as tabelas **Sales** e **Targets .**

1. Alterne para a visualização Modelo.
2. Na tabela **Date , oculte a coluna MonthKey** (defina **Is Hidden** como **Yes** ).
3. No painel do lado direito **Campos** , selecione a tabela **Data , clique com o botão direito do mouse na coluna Ano** e selecione **criar hierarquia** .
4. Renomeie a hierarquia recém-criada para **Fiscal** clicando com o botão direito e **Renomear** .
5. Adicione os dois campos restantes à hierarquia Fiscal selecionando-os no painel de campos, clicando com o botão direito do mouse, selecionando **Adicionar à hierarquia** -> **Fiscal** .

   - Trimestre
   - Mês

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image31.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image31.png)

6. Crie os dois relacionamentos de modelo a seguir:
   - **Data | Data** para **Vendas | Data do pedido**
   - **Data | Data** para **Metas | TargetMonth**
7. Oculte as duas colunas a seguir:
   - Vendas | Data do pedido
   - Alvos | TargetMonth

### **Tarefa 6: marque a tabela de datas**

Nesta tarefa, você marcará a tabela de **datas** como uma tabela de datas.

1. Mude para a visualização Relatório.
2. No painel **Campos** , selecione a tabela **Data (não o campo Data** ).
3. Na faixa contextual **Ferramentas de Tabela , no grupo Calendários** , clique em **Marcar como Tabela de Data** e selecione **Marcar como Tabela de Data** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image32.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image32.png)

4. Na janela **Marcar como Tabela de Data , na lista suspensa Coluna de Data** , selecione **Data** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image33.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image33.png)

5. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image34.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image34.png)

6. Salve o arquivo do Power BI Desktop.

   \*O Power BI Desktop agora entende que essa tabela define a data (hora). É importante quando se baseia em cálculos de inteligência de tempo. Você trabalhará com cálculos de inteligência de tempo no laboratório **Criar Cálculos DAX no Power BI Desktop, Parte 2 .\***

   _Observe que essa abordagem de design para uma tabela de datas é adequada quando você não tem uma tabela de datas em sua fonte de dados. Se você tiver um data warehouse, seria apropriado carregar dados de data de sua tabela de dimensão de data em vez de “redefinir” a lógica de data em seu modelo de dados._

## **Exercício 2: Criar Medidas**

Neste exercício, você criará e formatará várias medidas.

### **Tarefa 1: crie medidas simples**

Nesta tarefa, você criará medidas simples. Medidas simples agregam valores em uma única coluna ou contam linhas de uma tabela.

1. Na visualização Relatório, na **Página 2** , no painel **Campos , arraste o item Vendas | campo Preço unitário** no visual da matriz.

   _Os laboratórios usam uma notação abreviada para fazer referência a um campo. Ficará assim: **Vendas | Preço unitário** . Neste exemplo, **Vendas** é o nome da tabela e **Preço Unitário** é o nome do campo._

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image35.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image35.png)

   _Você deve se lembrar que no laboratório **Model Data in Power BI Desktop** , você define a coluna **Unit Price para resumir por Average** . O resultado que você vê no visual da matriz é o preço unitário médio mensal (soma dos valores dos preços unitários dividido pela contagem dos preços unitários)._

2. No painel de campos visuais (localizado abaixo do painel **Visualizações** ), no campo **Valores** bem/área, observe que **Preço unitário** está listado.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image36.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image36.png)

3. Clique na seta para baixo para **Preço unitário** e observe as opções de menu disponíveis.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image37.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image37.png)

   _Colunas numéricas visíveis permitem que os autores do relatório no tempo de design do relatório decidam como os valores da coluna serão resumidos (ou não). Isso pode resultar em relatórios inadequados. No entanto, alguns modeladores de dados não gostam de deixar as coisas ao acaso e optam por ocultar essas colunas e, em vez disso, expor a lógica de agregação definida em medidas. É a abordagem que você usará agora neste laboratório._

4. Para criar uma medida, no painel **Campos , clique com o botão direito do mouse na tabela Vendas** e selecione **Nova Medida** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image38.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image38.png)

5. Na barra de fórmulas, adicione a seguinte definição de medida:

   **DAX**

   ```
   Avg Price =
   ‎AVERAGE(Sales[Unit Price])
   ```

6. Adicione a medida de **preço médio** ao visual da matriz.
7. Observe que ela produz o mesmo resultado que a coluna **Unit Price** (mas com formatação diferente).
8. Na caixa **Valores** , abra o menu de contexto do campo **Preço médio** e observe que não é possível alterar a técnica de agregação.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image39.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image39.png)

   _Não é possível modificar o comportamento de agregação de uma medida._

9. Use as definições de arquivo de snippets para criar as cinco medidas a seguir para a tabela **Sales :**

   - Preço mediano
   - Preço mínimo
   - Preço máximo
   - Pedidos
   - Linhas de pedido

   _A função DISTINCTCOUNT() usada na medida **Orders** contará os pedidos apenas uma vez (ignorando duplicatas). A função COUNTROWS() usada na medida **Order Lines** opera em uma tabela._

   _Nesse caso, o número de pedidos é calculado contando os valores distintos da coluna **SalesOrderNumber** , enquanto o número de linhas do pedido é simplesmente o número de linhas da tabela (cada linha é uma linha de um pedido)._

10. Alterne para o modo de exibição de modelo e selecione várias vezes as quatro medidas de preço: **preço médio** , preço **máximo** , preço **mediano** e **preço mínimo** .
11. Para a seleção múltipla de medidas, configure os seguintes requisitos:

    - Defina o formato para duas casas decimais
    - Atribuir a uma pasta de exibição chamada **Preços**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image40.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image40.png)

12. Oculte a coluna **Preço unitário .**

    _A coluna **Preço unitário agora não está disponível para autores de relatórios.** Eles devem usar as medidas de preço que você adicionou ao modelo. Essa abordagem de design garante que os autores de relatórios não agreguem preços de forma inadequada, por exemplo, somando-os._

13. Selecione as medidas **Linhas** de Pedidos e **Pedidos** e configure os seguintes requisitos:

    - Defina o formato use o separador de milhares
    - Atribuir a uma pasta de exibição chamada **Contagens**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image41.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image41.png)

14. Na visualização Relatório, no poço/área **Valores** do visual da matriz, para o campo **Preço unitário** , clique em **X** para removê-lo.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image42.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image42.png)

15. Aumente o tamanho do visual da matriz para preencher a largura e a altura da página.
16. Adicione as cinco medidas a seguir ao visual da matriz:
    - Preço mediano
    - Preço mínimo
    - Preço máximo
    - Pedidos
    - Linhas de pedido
17. Verifique se os resultados parecem sensatos e estão formatados corretamente.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image43.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image43.png)

### **Tarefa 2: crie medidas adicionais**

Nesta tarefa, você criará medidas adicionais que usam fórmulas mais complexas.

1. Na visualização Relatório, selecione **Página 1** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image44.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image44.png)

2. Revise o visual da tabela, observando o total da coluna **Destino .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image45.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image45.png)

3. Selecione o visual da tabela e, no painel **Visualizações , remova o campo Destino** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image46.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image46.png)

4. Renomeie os **destinos |** Coluna de **destino como destinos | TargetAmount** .

   _Dica: Existem várias maneiras de renomear a coluna na exibição Relatório: No painel **Campos** , você pode clicar com o botão direito do mouse na coluna e selecionar **Renomear** — ou clicar duas vezes na coluna ou pressionar **F2** ._

   _Você está prestes a criar uma medida chamada **Target** . Não é possível ter uma coluna e uma medida na mesma tabela com o mesmo nome._

5. Crie a seguinte medida na tabela **Destinos :**

   **DAX**

   ```
   Target =

   IF(

   HASONEVALUE('Salesperson (Performance)'[Salesperson]),

   SUM(Targets[TargetAmount])

   )
   ```

   _A função HASONEVALUE() testa se um único valor na coluna **Vendedor é filtrado.** Quando true, a expressão retorna a soma dos valores de destino (apenas para esse vendedor). Quando false, BLANK é retornado._

6. Formate a medida **Target** para zero casas decimais.

   \*Dica: Você pode usar a faixa contextual **Ferramentas de medida .\***

7. Oculte a coluna **TargetAmount** .

   _Dica: Você pode clicar com o botão direito do mouse na coluna no painel **Campos** e selecionar **Ocultar** ._

8. Adicione a medida **Target** ao visual da tabela.
9. Observe que o total da coluna **Destino** agora está em BRANCO.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image47.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image47.png)

10. Use as definições de arquivo de snippets para criar as duas medidas a seguir para a tabela **Targets :**
    - Variação
    - Margem de variação
11. Formate a medida de **Variação** para zero casas decimais.
12. Formate a medida **Variance Margin** como porcentagem com duas casas decimais.
13. Adicione as medidas **Variance** e **Variance Margin** ao visual da tabela.
14. Redimensione o visual da tabela para que todas as colunas e linhas possam ser vistas.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image48.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image48.png)

    \*Embora pareça que todos os vendedores não estão atingindo a meta, lembre-se de que o visual da tabela ainda não foi filtrado por um período de tempo específico. Você produzirá relatórios de desempenho de vendas que filtram por um período de tempo selecionado pelo usuário no laboratório **Criar um Relatório no Power BI Desktop, Parte 1 .\***

15. No canto superior direito do painel **Campos** , recolha e expanda para abrir o painel.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image49.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image49.png)

    _Recolher e reabrir o painel redefine o conteúdo._

16. Observe que a tabela **Destinos** agora aparece no topo da lista.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image50.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/05-create-dax-calculations-in-power-bi-desktop_image50.png)

    _As tabelas que compreendem apenas medidas visíveis são listadas automaticamente no topo da lista._

### **Tarefa 3: Concluir**

Nesta tarefa, você concluirá o laboratório.

1. Salve o arquivo do Power BI Desktop.
2. Se você pretende iniciar o próximo laboratório, deixe o Power BI Desktop aberto.

   \*Você aprimorará o modelo de dados com cálculos mais avançados usando DAX no laboratório **Criar Cálculos DAX no Power BI Desktop, Parte 2 .\***

# Parabéns!
