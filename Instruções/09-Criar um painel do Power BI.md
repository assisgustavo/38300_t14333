# **Instruções de laboratório**

# **Criar um painel do Power BI**

**O tempo estimado para concluir o laboratório é de 45 minutos**

Neste laboratório, você criará o painel de **monitoramento de vendas .**

Neste laboratório, você aprenderá a:

- Fixar elementos visuais em um painel
- Use perguntas e respostas para criar blocos de painel

### **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. Preparar dados no Power BI Desktop
2. Carregar dados no Power BI Desktop
3. Dados do modelo no Power BI Desktop
4. Criar cálculos DAX no Power BI Desktop, Parte 1
5. Criar cálculos DAX no Power BI Desktop, Parte 2
6. Projetar um relatório no Power BI Desktop, Parte 1
7. Projetar um relatório no Power BI Desktop, Parte 2
8. Analise dados com visuais de IA
9. **Criar um painel do Power BI**
10. Aplicar segurança em nível de linha

## **Exercício 1: Criar um Painel**

Neste exercício, você criará o painel de **monitoramento de vendas .** O painel completo terá a seguinte aparência:

![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image1.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image1.png)

### **Tarefa 1: Começar – Entrar**

Nesta tarefa, você configurará o ambiente do laboratório entrando no Power BI.

*Importante: Se você já entrou no Power BI em um laboratório anterior, continue na próxima tarefa.*

1. Para abrir o Microsoft Edge, na barra de tarefas, clique no atalho do programa Microsoft Edge.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image2.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image2.png)
    
2. Na janela do navegador Microsoft Edge, navegue até **https://powerbi.microsoft.com** .
    
    *Dica: Você também pode usar o favorito do Serviço do Power BI na barra de favoritos do Microsoft Edge.*
    
3. Clique **em Entrar** (localizado no canto superior direito).
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image3.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image3.png)
    
4. Insira os detalhes da conta fornecidos a você.
5. Se solicitado a atualizar a senha, digite novamente a senha fornecida e, em seguida, digite e confirme uma nova senha.
    
    *Importante: Certifique-se de registrar sua nova senha.*
    
6. Conclua o processo de login.
7. Se solicitado pelo Microsoft Edge para permanecer conectado, clique em **Sim** .
8. Na janela do navegador Microsoft Edge, no serviço Power BI, no painel **Navegação** , expanda **Meu Workspace** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image4.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image4.png)
    
9. Deixe a janela do navegador Microsoft Edge aberta.

### **Tarefa 2: Começar – Abrir relatório**

Nesta tarefa, você configurará o ambiente do laboratório abrindo o relatório inicial.

*Importante: Se você continua no laboratório anterior (e concluiu esse laboratório com êxito), não conclua esta tarefa; em vez disso, continue a partir da próxima tarefa.*

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image5.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image5.png)
    
2. Para fechar a janela de introdução, no canto superior esquerdo da janela, clique em **X** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image6.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image6.png)
    
3. Se o Power BI Desktop não estiver conectado ao serviço do Power BI, no canto superior direito, clique em **Entrar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image7.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image7.png)
    
4. Conclua o processo de entrada usando a mesma conta usada para entrar no serviço do Power BI.
5. Para abrir o arquivo inicial do Power BI Desktop, clique na guia da faixa de opções **Arquivo** para abrir o modo de exibição de bastidores.
6. Selecione **Abrir relatório** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image8.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image8.png)
    
7. Clique **em Procurar relatórios** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image9.png)
    
8. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\08-create-power-bi-dashboard\Starter** .
9. Selecione o arquivo de **Análise de Vendas** .
10. Clique **em Abrir** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image10.png)
    
11. Feche todas as janelas informativas que possam ser abertas.
12. Para criar uma cópia do arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
13. Selecione **Salvar como** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image11.png)
    
14. Se solicitado a aplicar as alterações, clique em **Aplicar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image12.png)
    
15. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
16. Clique **em Salvar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image13.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image13.png)
    

### **Tarefa 3: Começar – Publicar o relatório**

Nesta tarefa, você configurará o ambiente do laboratório criando um conjunto de dados.

*Importante: Se você já publicou o relatório no laboratório **Criar um Relatório no Power BI Desktop, Parte 2** , continue na próxima tarefa.*

1. Na janela do navegador Microsoft Edge, no serviço Power BI, no painel **Navegação , na parte inferior, clique em Obter Dados** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image14.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image14.png)
    
2. No bloco **Arquivos** , clique em **Obter** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image15.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image15.png)
    
3. Clique no bloco **Arquivo local .**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image16.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image16.png)
    
4. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\08-create-power-bi-dashboard\Solution** .
5. Selecione o arquivo **Sales Analysis.pbix** e clique em **Abrir** .
6. Se solicitado a substituir o conjunto de dados, clique em **Substituir** .

### **Tarefa 4: crie um painel**

Nesta tarefa, você criará o painel de **monitoramento de vendas .** Você fixará um visual do relatório e adicionará um bloco com base em um URI de dados de imagem e usará perguntas e respostas para criar um bloco.

1. Na janela do navegador Microsoft Edge, no serviço Power BI, abra o relatório de **Análise de Vendas** .
2. Na página **Visão geral** , defina a segmentação de **ano** como **FY2020** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image17.png)
    
3. Defina a segmentação de **região** para **Selecionar tudo** .
    
    *Ao fixar visuais em um painel, eles usarão o contexto de filtro atual. Uma vez fixado, o contexto do filtro não pode ser alterado. Para filtros baseados em tempo, é melhor usar uma segmentação de data relativa (ou perguntas e respostas usando uma pergunta baseada em tempo relativo).*
    
4. Para criar um painel e fixar um visual, passe o cursor sobre o visual **Margem de vendas e lucro por mês** (coluna/linha).
5. No canto inferior direito, clique no alfinete.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image18.png)
    
6. Na janela **Pin to Dashboard , na caixa Dashboard Name** , insira **Sales Monitoring** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image19.png)
    
7. Clique **em Fixar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image20.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image20.png)
    
8. Abra o painel de **navegação** , selecione **meu espaço** de trabalho e abra o painel de **monitoramento de vendas .**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image21.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image21.png)
    
9. Observe que o painel tem um único bloco.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image22.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image22.png)
    
10. Para adicionar um bloco com base em uma pergunta, no canto superior esquerdo do painel, clique em **Fazer uma pergunta sobre seus dados** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image23.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image23.png)
    
    *Você pode usar o recurso de perguntas e respostas para fazer uma pergunta, e o Power BI responderá com um visual.*
    
11. Clique em qualquer uma das perguntas sugeridas abaixo da caixa de perguntas e respostas, nas caixas azuis.
12. Revise a resposta.
13. Remova todo o texto da caixa de perguntas e respostas.
14. Na caixa de perguntas e respostas, insira o seguinte: **Vendas YTD**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image24.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image24.png)
    
15. Observe a resposta de **(Blank)** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image25.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image25.png)
    
    *Você deve se lembrar de ter adicionado a medida **Sales YTD** no laboratório **Criar cálculos DAX no Power BI Desktop, Parte 2 .** Essa medida é uma expressão de inteligência de tempo e, portanto, requer um filtro na tabela **Data** para produzir um resultado.*
    
16. Estenda a pergunta com: **no ano FY2020** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image26.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image26.png)
    
17. Observe que a resposta agora é **de US$ 33 milhões** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image27.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image27.png)
    
18. Para fixar a resposta no painel, no canto superior direito, clique em **Fixar Visual** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image28.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image28.png)
    
19. Quando solicitado a fixar o bloco no painel, clique em **Fixar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image29.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image29.png)
    
20. Para retornar ao painel, no canto superior esquerdo, clique em **Sair de perguntas e respostas** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image30.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image30.png)
    
21. Para adicionar o logotipo da empresa, na barra de menus, clique em **Editar** e selecione **Adicionar um bloco** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image31.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image31.png)
    
    *O uso dessa técnica para adicionar um bloco de painel permite embelezar seu painel com mídia, incluindo conteúdo da Web, imagens, caixas de texto com formatação avançada e vídeo (usando links do YouTube ou do Vimeo).*
    
22. No painel **Adicionar um** bloco (localizado à direita), selecione o bloco **Imagem .**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image32.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image32.png)
    
23. Clique **em Avançar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image33.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image33.png)
    
24. No painel **Add Image Tile , na caixa URL** , insira a URL completa encontrada no arquivo **D:\PL300\Resources\AdventureWorksLogo_DataURL.txt** .
    
    *Você pode incorporar uma imagem usando seu URL ou pode usar um URL de dados, que incorpora conteúdo inline.*
    
25. Na parte inferior do painel, clique em **Aplicar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image34.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image34.png)
    
26. Para redimensionar o bloco do logotipo, arraste o canto inferior direito e redimensione o bloco para ter uma unidade de largura e duas unidades de altura.
    
    *Os tamanhos dos blocos são restringidos em uma forma retangular. Só é possível redimensionar em múltiplos da forma retangular.*
    
27. Organize os blocos para que o logotipo apareça no canto superior esquerdo, com o bloco **Vendas YTD** abaixo dele e o bloco **Vendas, Margem de Lucro** à direita.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image35.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image35.png)
    

### **Tarefa 5: editar detalhes do bloco**

Nesta tarefa, você editará os detalhes de dois blocos.

1. Passe o cursor sobre o bloco **Vendas YTD** e, no canto superior direito do bloco, clique nas reticências e selecione **Editar detalhes** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image36.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image36.png)
    
2. No painel **Detalhes** do bloco (localizado à direita), na caixa **Legenda** , insira **FY2020** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image37.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image37.png)
    
3. Clique **em Aplicar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image38.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image38.png)
    
4. Observe que o bloco **Vendas YTD** exibe uma legenda.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image39.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image39.png)
    
5. Edite os detalhes do bloco para o bloco **Vendas, Margem de Lucro** .
6. No painel **Detalhes do bloco, na seção Funcionalidade** , marque **Exibir hora da última atualização** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image40.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image40.png)
    
7. Clique **em Aplicar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image41.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image41.png)
    
8. Observe que o bloco descreve a hora da última atualização (que é feita ao carregar o modelo de dados no Power BI Desktop).
    
    *Você atualizará o conjunto de dados no próximo exercício. Normalmente, isso seria feito usando a atualização agendada, caso em que o Power BI usaria um gateway para se conectar ao banco de dados do SQL Server. No entanto, devido a restrições na configuração da sala de aula, não há gateway. Assim, você abrirá o Power BI Desktop, realizará uma atualização manual de dados e, em seguida, carregará o arquivo em seu workspace.*
    

## **Exercício 2: Atualize o conjunto de dados**

Neste exercício, você primeiro carregará os dados do pedido de vendas de junho de 2020 no banco de dados **AdventureWorksDW2020** . Em seguida, você abrirá seu arquivo do Power BI Desktop, realizará uma atualização de dados e carregará o arquivo em seu workspace.

### **Tarefa 1: atualize o banco de dados do laboratório**

Nesta tarefa, você executará um script do PowerShell para atualizar dados no banco de dados **AdventureWorksDW2020** .

1. No Explorador de Arquivos, dentro da pasta **D:\PL300\Setup** , clique com o botão direito do mouse no **arquivo UpdateDatabase-2-AddSales.ps1** e selecione **Executar com PowerShell** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image46.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image46.png)
    
2. Se solicitado a alterar a política de execução, pressione **A** .
3. Quando solicitado a pressionar qualquer tecla para fechar, pressione **Enter** novamente.
    
    *O banco de dados **AdventureWorksDW2020** agora inclui pedidos de vendas feitos em junho de 2020.*
    

### **Tarefa 2: atualize o arquivo do Power BI Desktop**

Nesta tarefa, você abrirá o arquivo do Power BI Desktop da **Análise de Vendas** , realizará uma atualização de dados e, em seguida, carregará o arquivo no workspace da **Análise de Vendas .**

1. No arquivo do Power BI Desktop, no painel **Campos , clique com o botão direito do mouse na tabela Vendas** e selecione **Atualizar Dados** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image47.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image47.png)
    
2. Quando a atualização for concluída, salve o arquivo do Power BI Desktop.
3. Para publicar o arquivo em seu workspace, na guia **Home** da faixa de opções, de dentro do grupo **Compartilhar** , clique em **Publicar** e, em seguida, clique em **Selecionar** para publicar.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image48.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image48.png)
    
4. Quando solicitado a substituir o conjunto de dados, clique em **Substituir** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image49.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image49.png)
    
    *O conjunto de dados no serviço do Power BI agora tem dados de vendas de junho de 2020.*
    
5. Feche o Power BI Desktop.

## **Exercício 3: Revise o Painel**

Neste exercício, você revisará o painel para observar as vendas atualizadas.

### **Tarefa 1: revise o painel**

Nesta tarefa, você revisará o painel para observar as vendas atualizadas.

1. Na janela do navegador Microsoft Edge, no serviço Power BI, revise o painel **Monitoramento de Vendas .**
2. No bloco **Vendas, Margem de Lucro** , na legenda, observe que os dados foram atualizados **AGORA** .
3. Observe também que agora há uma coluna para **2020 Jun** .
    
    *Se você não vir os dados de junho de 2020, talvez seja necessário pressionar **F5** para recarregar o navegador da Web.*
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image50.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/09-create-power-bi-dashboard_image50.png)
    
4. Para fechar o painel, clique em **Fechar** .

# Parabéns!