# **Aplicar segurança em nível de linha**

**O tempo estimado para concluir o laboratório é de 45 minutos**

Neste laboratório, você aplicará a segurança em nível de linha para garantir que um vendedor só possa analisar os dados de vendas da(s) região(ões) atribuída(s).

Neste laboratório, você aprenderá a:

- Aplicar segurança em nível de linha

### **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. Preparar dados no Power BI Desktop
2. Carregar dados no Power BI Desktop
3. Projetar um modelo de dados no Power BI
4. Criar cálculos DAX no Power BI Desktop, Parte 1
5. Criar cálculos DAX no Power BI Desktop, Parte 2
6. Projetar um relatório no Power BI Desktop, Parte 1
7. Projetar um relatório no Power BI Desktop, Parte 2
8. Analise dados com visuais de IA
9. Criar um painel do Power BI
10. **Aplicar segurança em nível de linha**

## **Exercício 1: aplicar a segurança em nível de linha**

Neste exercício, você aplicará a segurança em nível de linha para garantir que um vendedor só possa ver as vendas feitas na(s) região(ões) atribuída(s).

### **Tarefa 1: comece**

Nesta tarefa, você configurará o ambiente para o laboratório.

_Importante: Se você continua no laboratório anterior (e concluiu esse laboratório com êxito), não conclua esta tarefa; em vez disso, continue a partir da próxima tarefa._

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image1.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image1.png)

2. Para fechar a janela de introdução, no canto superior esquerdo da janela, clique em **X** .

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image2.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image2.png)

3. Para abrir o arquivo inicial do Power BI Desktop, clique na guia da faixa de opções **Arquivo** para abrir o modo de exibição de bastidores.
4. Selecione **Abrir relatório** .

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image3.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image3.png)

5. Clique **em Procurar relatórios** .

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image4.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image4.png)

6. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\10-row-level-security\Starter** .
7. Selecione o arquivo de **Análise de Vendas** .
8. Clique **em Abrir** .

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image5.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image5.png)

9. Feche todas as janelas informativas que possam ser abertas.
10. Para criar uma cópia do arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
11. Selecione **Salvar como** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image6.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image6.png)

12. Se solicitado a aplicar as alterações, clique em **Aplicar** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image7.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image7.png)

13. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
14. Clique **em Salvar** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image8.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image8.png)

### **Tarefa 2: aplicar a segurança em nível de linha**

Nesta tarefa, você aplicará a segurança em nível de linha para garantir que um vendedor possa ver apenas as vendas feitas em sua(s) região(ões) atribuída(s).

1. Mude para a visualização de dados.

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image20.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image20.png)

2. No painel **Campos** , selecione a tabela **Vendedor (Desempenho) .**
3. Revise os dados, observando que Michael Blythe (EmployeeKey 281) tem um valor UPN de: **[michael-blythe@adventureworks.com](mailto:michael-blythe@adventureworks.com)**

   _Lembre-se de que Michael Blythe é atribuído a três regiões de vendas: Nordeste dos EUA, Central dos EUA e Sudeste dos EUA._

4. Mude para a visualização Relatório.
5. Na guia **Modelagem , no grupo Segurança** , clique em **Gerenciar Funções** .

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image21.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image21.png)

6. Na janela **Gerenciar Funções** , clique em **Criar** .

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image22.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image22.png)

7. Na caixa, substitua o texto selecionado pelo nome da função: **Vendedores** e pressione **Enter** .

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image23.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image23.png)

8. Para atribuir um filtro, para a tabela **Vendedor (Desempenho)** , clique no caractere de reticências (…) e selecione **Adicionar Filtro | [UPN]** .

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image24.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image24.png)

9. Na caixa **Expressão DAX do Filtro de Tabela** , modifique a expressão substituindo **“Value”** por **USERPRINCIPALNAME()** .

   ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image25.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image25.png)

   _USERPRINCIPALNAME() é uma função Data Analysis Expressions (DAX) que retorna o nome do usuário autenticado. Isso significa que a tabela **Vendedor (Desempenho)** filtrará pelo Nome Principal do Usuário (UPN) do usuário que está consultando o modelo._

10. Clique **em Salvar** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image26.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image26.png)

11. Para testar a função de segurança, na guia **Modelagem , de dentro do grupo Segurança** , clique em **Exibir como** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image27.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image27.png)

12. Na janela **Exibir como funções , marque o item Outro usuário** e, na caixa correspondente, digite: **[michael-blythe@adventureworks.com](mailto:michael-blythe@adventureworks.com)**
13. Verifique a função **Vendedores** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image28.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image28.png)

    _Essa configuração resulta no uso da função **Vendedores** e na representação do usuário com o nome de seu Michael Blythe._

14. Clique **em OK** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image29.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image29.png)

15. Observe o banner amarelo acima da página do relatório, descrevendo o contexto de segurança do teste.

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image30.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image30.png)

16. No visual da tabela, observe que apenas o vendedor **Michael Blythe** está listado.

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image31.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image31.png)

17. Para interromper o teste, no lado direito do banner amarelo, clique em **Parar visualização** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image32.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image32.png)

    _Quando o arquivo do Power BI Desktop for publicado no serviço do Power BI, você precisará concluir uma tarefa de pós-publicação para mapear entidades de segurança para a função **Vendedores** . Você não fará isso neste laboratório._

18. Para excluir a função, na guia **Modelagem , dentro do grupo Segurança** , clique em **Gerenciar Funções** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image33.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image33.png)

19. Na janela **Gerenciar Funções** , clique em **Excluir** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image34.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image34.png)

20. Quando solicitado a confirmar a exclusão, clique em **Sim, Excluir** .
21. Clique **em Salvar** .

    ![https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image35.png](https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image35.png)

### **Tarefa 3: Concluir**

Nesta tarefa, você concluirá o laboratório.

1. Salve o arquivo do Power BI Desktop.
