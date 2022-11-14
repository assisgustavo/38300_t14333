# **Instruções de laboratório**

# Projetar um relatório no Power BI Desktop, Parte 1

**O tempo estimado para concluir o laboratório é de 45 minutos.**

Neste laboratório, você criará um relatório de três páginas. Em seguida, você o publicará no Power BI, onde abrirá e interagirá com o relatório.

Neste laboratório, você aprenderá a:

- Projete um relatório
- Configurar campos visuais e propriedades de formato

### **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. Preparar dados no Power BI Desktop
2. Carregar dados no Power BI Desktop
3. Projetar um modelo de dados no Power BI
4. Criar cálculos DAX no Power BI Desktop, Parte 1
5. Criar cálculos DAX no Power BI Desktop, Parte 2
6. **Projetar um relatório no Power BI Desktop, Parte 1**
7. Projetar um relatório no Power BI Desktop, Parte 2
8. Analise dados com visuais de IA
9. Criar um painel do Power BI
10. Aplicar segurança em nível de linha

## **Exercício 1: Criar um Relatório**

Neste exercício, você criará um relatório de três páginas chamado **Relatório de vendas** .

### **Tarefa 1: Começar – Entrar**

Nesta tarefa, você configurará o ambiente do laboratório entrando no Power BI.

_Importante: Se você já entrou no Power BI, continue na próxima tarefa._

1. Para abrir o Microsoft Edge, na barra de tarefas, clique no atalho do programa Microsoft Edge.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image1.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image1.png)

2. Na janela do navegador Microsoft Edge, navegue até **https://powerbi.microsoft.com** .

   _Dica: Você também pode usar o favorito do Serviço do Power BI na barra de favoritos do Microsoft Edge._

3. Clique **em Entrar** (localizado no canto superior direito).

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image2.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image2.png)

4. Conclua o processo de login.
5. Se solicitado pelo Microsoft Edge para permanecer conectado, clique em **Sim** .
6. Deixe a janela do navegador Microsoft Edge aberta.

### **Tarefa 2: Começar – Ativar mapas e visuais de mapa preenchidos**

Nesta tarefa, você habilitará os visuais de mapa e de mapa preenchido no ambiente para o laboratório, atualizando as configurações globais no Power BI Desktop e as configurações de integração no portal de administração do Power BI.

1. No Power BI Desktop, navegue até **Opções > Opções e configurações > GlobalUsar visuais de mapa e mapa preenchido**

   e marque a caixa para

   .

![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image103b.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image103b.png)

1. Para abrir o portal de administração do Power BI, no canto superior direito do navegador Edge, clique no ícone **Configurações .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image101.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image101.png)

2. Selecione **Portal do administrador** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image102.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image102.png)

3. Role a página até as configurações de integração. Clique na seta para expandir a opção Mapa e visuais de mapa preenchidos.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image103.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image103.png)

4. Defina a opção Mapa e visuais de mapa preenchidos como **Ativado** .
5. Clique em **Aplicar** , para aplicar as alterações.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image104.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image104.png)

6. Uma mensagem aparecerá no canto superior direito do navegador informando que as alterações nas configurações do locatário serão aplicadas nos próximos 15 minutos.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image105.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image105.png)

7. Deixe a janela do navegador Microsoft Edge aberta.

### **Tarefa 3: Começar – Abrir relatório**

Nesta tarefa, você configurará o ambiente do laboratório abrindo o relatório inicial.

_Importante: Se você continua no laboratório anterior (e concluiu esse laboratório com êxito), não conclua esta tarefa; em vez disso, continue a partir da próxima tarefa._

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image3.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image3.png)

2. Para fechar a janela de introdução, no canto superior esquerdo da janela, clique em **X** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image4.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image4.png)

3. Para entrar no serviço do Power BI, no canto superior direito, clique em **Entrar** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image5.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image5.png)

4. Conclua o processo de entrada usando a mesma conta usada para entrar no serviço do Power BI.
5. Para abrir o arquivo inicial do Power BI Desktop, clique na guia da faixa de opções **Arquivo** para abrir o modo de exibição de bastidores.
6. Selecione **Abrir relatório** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image6.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image6.png)

7. Clique **em Procurar relatórios** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image7.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image7.png)

8. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\06-design-report-in-power-bi-desktop\Starter** .
9. Selecione o arquivo de **Análise de Vendas** .
10. Clique **em Abrir** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image8.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image8.png)

11. Feche todas as janelas informativas que possam ser abertas.
12. Para criar uma cópia do arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
13. Selecione **Salvar como** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image9.png)

14. Se solicitado a aplicar as alterações, clique em **Aplicar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image10.png)

15. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
16. Clique **em Salvar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image11.png)

### **Tarefa 4: Projetar página 1**

Nesta tarefa, você projetará a primeira página do relatório. Quando você tiver concluído o design, a página terá a seguinte aparência:

![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image12.png)

1. No Power BI Desktop, para renomear a página, no canto inferior esquerdo, clique com o botão direito do mouse em **Página 1** e selecione **Renomear** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image13.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image13.png)

   _Dica: Você também pode clicar duas vezes no nome da página para renomeá-la._

2. Renomeie a página como **Visão geral** e pressione **Enter** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image14.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image14.png)

3. Para adicionar uma imagem, na guia **Inserir** da faixa de opções, de dentro do grupo **Elementos** , clique em **Imagem** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image15.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image15.png)

4. Na janela **Abrir , navegue até a pasta D:\PL300\Resources** .
5. Selecione o arquivo **AdventureWorksLogo.jpg** e clique em **Abrir** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image16.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image16.png)

6. Arraste a imagem para posicioná-la no canto superior esquerdo e também arraste os marcadores de guia para redimensioná-la.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image17.png)

7. Para adicionar uma segmentação de dados, primeiro desmarque a imagem clicando em uma área vazia da página do relatório.
8. No painel **Campos , selecione Data | Campo Ano** (não o nível **Ano** da hierarquia).

   _Os laboratórios usam uma notação abreviada para fazer referência a um campo. Será assim: **Data | Ano** . Neste exemplo, **Data** é o nome da tabela e **Ano** é o nome do campo._

9. Observe que uma tabela de valores de ano foi adicionada à página do relatório.
10. Para converter o visual de uma tabela em uma segmentação de dados, no painel **Visualizações , selecione a segmentação** de dados .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image18.png)

11. Para converter a segmentação de uma lista em uma lista suspensa, no canto superior direito da segmentação, clique na seta para baixo e selecione Lista **suspensa** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image19.png)

12. Redimensione e posicione o slicer para que fique abaixo da imagem e tenha a mesma largura da imagem.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image20.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image20.png)

13. Na segmentação de **ano** , abra a lista suspensa, selecione **FY2020** e, em seguida, recolha a lista suspensa.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image21.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image21.png)

    _A página do relatório agora é filtrada por ano **FY2020** ._

14. Desmarque a segmentação clicando em uma área vazia da página do relatório.
15. Crie uma segunda segmentação, com base na **região | Campo de região** (não o nível de **região** da hierarquia).
16. Deixe o slicer como uma lista e, em seguida, redimensione e posicione o slicer abaixo do slicer **Year** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image22.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image22.png)

17. Desmarque a segmentação clicando em uma área vazia da página do relatório.
18. Para adicionar um gráfico à página, no painel **Visualizações** , clique no tipo de visual **Gráfico de linhas e colunas empilhadas .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image26.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image26.png)

19. Redimensione e posicione o visual para que fique à direita do logotipo e preencha a largura da página do relatório.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image27.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image27.png)

20. Arraste e solte os seguintes campos no visual:
    - Data | Mês
    - Vendas | Vendas
21. No painel de campos visuais (não no painel **Campos** —o painel de campos visuais está localizado abaixo do painel **Visualizações** ), observe que os campos são atribuídos aos poços/áreas **do eixo X** e da **coluna y .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image28_N.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image28_N.png)

    _Ao arrastar os campos para um visual, eles serão adicionados aos poços/áreas padrão. Para maior precisão, você pode arrastar os campos diretamente para os poços/áreas, como fará a seguir._

22. No painel **Campos , arraste o item Vendas |** Campo **de margem de lucro** no poço/área **do eixo y da linha .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image29.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image29.png)

23. Observe que o visual tem apenas 11 meses.

    _O último mês do ano, junho de 2020, não tem vendas (ainda). Por padrão, o visual eliminou meses com vendas em BRANCO. Agora você configurará o visual para mostrar todos os meses._

24. No painel de campos visuais, no poço/área **do eixo X , para o campo Mês** , clique na seta para baixo e selecione **Mostrar itens sem dados** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image30.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image30.png)

25. Observe que o mês de **junho de 2020** agora aparece.
26. Desmarque o gráfico clicando em uma área vazia da página do relatório.
27. Para adicionar um gráfico à página, no painel **Visualizações** , clique no tipo de visual **Mapa .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image31.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image31.png)

28. Redimensione e posicione o visual para que fique abaixo do gráfico de colunas/linhas e preencha metade da largura do gráfico acima.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image32.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image32.png)

29. Adicione os seguintes campos aos poços/áreas visuais:
    - Local: **Região | País**
    - Legenda: **Produto | Categoria**
    - Tamanho: **Vendas | Vendas**
30. Desmarque o gráfico clicando em uma área vazia da página do relatório.
31. Para adicionar um gráfico à página, no painel **Visualizações** , clique no tipo de visual **Gráfico de Barras Empilhadas .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image33.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image33.png)

32. Redimensione e posicione o visual para que ele preencha o espaço restante da página do relatório.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image34.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image34.png)

33. Adicione os seguintes campos aos poços/áreas visuais:
    - Eixo: **Produto | Categoria**
    - Valor: **Vendas | Quantidade**
34. Para formatar o visual, abra o painel **Formatar .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image35.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image35.png)

35. Expanda o grupo **Barras** e, em seguida, o grupo **Cores** e, em seguida, defina a propriedade **Default Color** para uma cor adequada (para complementar o gráfico de colunas/linhas).
36. Defina a propriedade **Data Labels como On** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image36.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image36.png)

37. Salve o arquivo do Power BI Desktop.

    _O design da primeira página está agora completo._

### **Tarefa 5: Projetar página 2**

Nesta tarefa, você projetará a segunda página do relatório. Quando você tiver concluído o design, a página terá a seguinte aparência:

![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image37.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image37.png)

_Importante: quando instruções detalhadas já tiverem sido fornecidas nos laboratórios, as etapas do laboratório fornecerão instruções mais concisas. Se você precisar de instruções detalhadas, consulte outras tarefas neste laboratório._

1. Para criar uma nova página, no canto inferior esquerdo, clique no ícone de adição.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image38.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image38.png)

2. Renomeie a página para **Lucro** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image39.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image39.png)

3. Adicionar um slicer com base na **região | Campo região** .
4. Use o painel **Formato** para habilitar a opção “Selecionar tudo” (no grupo **Seleção** ).
5. Redimensione e posicione a segmentação de dados de modo que fique no lado esquerdo da página do relatório e tenha cerca de metade da altura da página.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image40.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image40.png)

6. Adicione um visual de matriz e redimensione-o e posicione-o para que preencha o espaço restante da página do relatório

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image41.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image41.png)

7. Adicionar a **data | Hierarquia fiscal** para a matriz **Linhas** bem/área.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image42.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image42.png)

8. Adicione os cinco campos da tabela **Vendas** a seguir ao poço/área **Valores :**

   - Pedidos (da pasta **Counts )**
   - Vendas
   - Custo
   - Lucro
   - Margem de lucro

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image43.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image43.png)

9. No painel **Filtros** (localizado à esquerda do painel **Visualizações** ), observe o poço/área **Filtrar nesta página** (talvez seja necessário rolar para baixo).

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image44.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image44.png)

10. No painel **Campos , arraste o Produto | Categoria** no poço/área **Filtrar nesta página .**
11. Dentro do cartão de filtro, no canto superior direito, clique na seta para recolher o cartão.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image45.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image45.png)

    _Os campos adicionados ao painel **Filtros podem obter o mesmo resultado que uma segmentação de dados.** Uma diferença é que eles não ocupam espaço na página do relatório. Outra diferença é que eles podem ser configurados para atingir requisitos de filtragem mais sofisticados._

12. Adicione cada um dos campos da tabela **Produto a seguir à área/ filtro Filtrar nesta página** , recolhendo cada um deles, diretamente abaixo do cartão **Categoria** :

    - Subcategoria
    - produtos
    - Cor

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image46.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image46.png)

13. Salve o arquivo do Power BI Desktop.

    _O design da segunda página está agora completo._

### **Tarefa 6: Projetar página 3**

Nesta tarefa, você projetará a terceira e última página do relatório. Quando você tiver concluído o design, a página terá a seguinte aparência:

![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image47.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image47.png)

1. Crie uma nova página e renomeie-a como **Meu Desempenho** .
2. Para simular o desempenho de filtros de segurança em nível de linha, arraste o **item Vendedor (Desempenho) | Campo de vendedor** para os filtros de nível de página no painel de filtros.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image999.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image999.png)

3. Selecione **Michael Blythe** . Os dados na página do relatório **Meu desempenho** agora serão filtrados para exibir dados apenas de Michael Blythe.
4. Adicione uma segmentação suspensa com base na **Data | Ano** e, em seguida, redimensione-o e posicione-o no canto superior esquerdo da página.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image49.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image49.png)

5. Na segmentação de dados, defina a página para filtrar por **FY2019** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image50.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image50.png)

6. Adicione um visual **Cartão de várias linhas** e, em seguida, redimensione e reposicione-o para que fique à direita da segmentação de dados e preencha a largura restante da página.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image51.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image51.png)

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image52.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image52.png)

7. Adicione os quatro campos a seguir ao visual:
   - Vendas | Vendas
   - Alvos | Alvo
   - Alvos | Variação
   - Alvos | Margem de variação
8. Formate o visual:

   - No grupo de **valores de Callout** , aumente a propriedade **Text Size** para **28pt**
   - No grupo Plano de **fundo** , defina a **Cor** para uma cor cinza claro

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image53.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image53.png)

9. Adicione um visual de **Gráfico de Barras Agrupadas** e, em seguida, redimensione e posicione-o para que fique abaixo do visual de cartão de várias linhas e preencha a altura restante da página e metade da largura do visual de cartão de várias linhas.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image54.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image54.png)

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image55.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image55.png)

10. Adicione os seguintes campos aos poços/áreas visuais:

    - Eixo: **Data | Mês**
    - Valor: **Vendas | Vendas** e **Metas | Alvo**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image56.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image56.png)

11. Para criar uma cópia do visual, pressione **Ctrl+C** e, em seguida, pressione **Ctrl+V** .
12. Posicione o novo visual à direita do visual original.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image57.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image57.png)

13. Para modificar o tipo de visualização, no painel **Visualizações** , selecione **Gráfico de Colunas Agrupadas** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image58.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image58.png)

    _Agora é possível ver os mesmos dados expressos por dois tipos de visualização diferentes. Esse não é um bom uso do layout de página, no entanto, você o aprimorará no laboratório Criar **um Relatório no Power BI Desktop, Parte 2** , sobrepondo os visuais. Ao adicionar botões à página, você permitirá que o usuário do relatório determine qual dos dois visuais está visível._

    _O design da terceira – e última – página está agora completo._

### **Tarefa 7: publique o relatório**

Nesta tarefa você publicará o relatório.

1. Selecione a página **Visão geral** .
2. Salve o arquivo do Power BI Desktop.
3. Na guia da faixa de opções **Home , de dentro do grupo Compartilhar** , clique em **Publicar** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image59.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image59.png)

4. Na janela **Publicar no Power** BI, observe que **Meu Workspace** está selecionado.
5. Para publicar o relatório, clique em **Selecionar** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image60.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image60.png)

6. Quando a publicação for bem-sucedida, clique em **Entendi** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image61.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image61.png)

7. Deixe o Power BI Desktop aberto.

   _Você explorará o relatório no serviço do Power BI no próximo exercício._

## **Exercício 2: Explore o Relatório**

Neste exercício, você explorará o relatório que foi publicado no Power BI.

### **Tarefa 1: explore o relatório**

Nesta tarefa, você explorará o relatório que foi publicado no Power BI.

1. Na janela do navegador Microsoft Edge, no serviço Power BI, no painel **Navegação** (localizado à esquerda e pode ser recolhido), expanda **Meu Espaço** de Trabalho .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image62.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image62.png)

2. Revise o conteúdo do espaço de trabalho, observando o relatório de **análise de vendas** e o conjunto de dados.

   _Quando você publicou o arquivo do Power BI Desktop, o modelo de dados foi publicado como um conjunto de dados._

   _Se você não o vir, pressione **F5** para recarregar o navegador e expanda o espaço de trabalho novamente._

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image63.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image63.png)

3. Para abrir o relatório, clique no relatório **Análise de vendas** .
4. À esquerda, no painel **Páginas , selecione a página Visão geral** .

   **\*Observação** : se você vir um erro de que o visual do mapa está desativado, atualize seu navegador.\*

5. Na segmentação de **regiões** , enquanto pressiona a tecla **Ctrl** , selecione várias regiões.
6. No gráfico de colunas/linhas, selecione qualquer coluna de mês para filtrar a página.
7. Enquanto pressiona a tecla **Ctrl** , selecione um mês adicional.

   _Por padrão, a filtragem cruzada filtra todos os outros visuais da página._

8. Observe que o gráfico de barras é filtrado e destacado, com a parte em negrito das barras representando os meses filtrados.
9. Passe o cursor sobre o visual do gráfico de barras e, no canto superior direito, passe o cursor sobre o ícone de filtro.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image64.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image64.png)

   _O ícone de filtro permite que você entenda todos os filtros aplicados ao visual, incluindo segmentações e filtros cruzados de outro visual._

10. Passe o cursor sobre uma barra e observe as informações da dica de ferramenta.
11. Para desfazer o filtro cruzado, no gráfico de colunas/linhas, clique em uma área vazia do visual.
12. Passe o cursor sobre o visual do mapa e, no canto superior direito, clique no ícone do **modo de foco .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image65.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image65.png)

    _O modo de foco amplia o visual para o tamanho da página inteira._

13. Passe o cursor sobre diferentes segmentos dos gráficos de barras para revelar dicas de ferramentas.
14. Para retornar à página do relatório, no canto superior esquerdo, clique em **Voltar ao relatório** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image66.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image66.png)

15. Passe o cursor sobre o visual do mapa novamente e, no canto superior direito, clique nas reticências (…) e observe as opções do menu.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image67.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image67.png)

16. Experimente cada uma das opções, exceto **Bate-papo no Teams** .
17. À esquerda, no painel **Páginas , selecione a página Lucro** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image68.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image68.png)

18. Observe que a segmentação de **região** tem uma seleção diferente da segmentação de **região na página Visão geral** .

    \*As segmentações não estão sincronizadas. Você modificará o design do relatório para garantir que eles sejam sincronizados entre as páginas no laboratório **Criar um Relatório no Power BI Desktop, Parte 2 .\***

19. No painel **Filtros** (localizado à direita), expanda um cartão de filtro e aplique alguns filtros.

    _O painel **Filtros** permite definir mais filtros do que poderia caber em uma página como segmentações._

20. No visual de matriz, use o botão de adição (+) para detalhar a hierarquia **fiscal .**
21. Selecione a página **Meu desempenho** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image69.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image69.png)

22. No canto superior direito da barra de menus, clique em **Exibir** e selecione **Tela inteira** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image70.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image70.png)

23. Interaja com a página modificando a segmentação e filtrando a página de forma cruzada.
24. Na parte inferior da janela, observe os comandos para mudar de página, navegar para trás ou para frente entre as páginas ou para sair do modo de tela cheia.
25. Clique no ícone esquerdo para sair do modo de tela cheia.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image71.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image71.png)

### **Tarefa 2: Concluir**

Nesta tarefa, você concluirá o laboratório.

1. Para retornar ao seu espaço de trabalho, no banner da página da Web da janela, clique em **Meu Espaço** de Trabalho .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image72.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image72.png)

2. Deixe a janela do navegador Microsoft Edge aberta.

   \*Você aprimorará o design do relatório com recursos avançados no laboratório **Criar um Relatório no Power BI Desktop, Parte 2 .\***

# Parabéns!
