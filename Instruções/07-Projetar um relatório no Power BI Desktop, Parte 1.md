# **Instruções de laboratório**

# Projetar um relatório no Power BI Desktop, Parte 2

**O tempo estimado para concluir o laboratório é de 45 minutos.**

Neste laboratório, você aprimorará a **Análise de vendas** com recursos avançados de design.

Neste laboratório, você aprenderá a:

- Sincronizar segmentações
- Criar uma página de detalhamento
- Aplicar formatação condicional
- Criar e usar marcadores

### **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. Preparar dados no Power BI Desktop
2. Carregar dados no Power BI Desktop
3. Projetar um modelo de dados no Power BI
4. Criar cálculos DAX no Power BI Desktop, Parte 1
5. Criar cálculos DAX no Power BI Desktop, Parte 2
6. Projetar um relatório no Power BI Desktop, Parte 1
7. **Projetar um relatório no Power BI Desktop, Parte 2**
8. Analise dados com visuais de IA
9. Criar um painel do Power BI
10. Aplicar segurança em nível de linha

## **Exercício 1: configurar segmentações de sincronização**

Neste exercício, você sincronizará as segmentações de página do relatório.

### Tarefa 1: Começar – Entrar

Nesta tarefa, você configurará o ambiente do laboratório entrando no Power BI.

*Importante: Se você já entrou no Power BI, continue na próxima tarefa.*

1. Para abrir o Microsoft Edge, na barra de tarefas, clique no atalho do programa Microsoft Edge.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image1.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image1.png)
    
2. Na janela do navegador Microsoft Edge, navegue até **https://powerbi.microsoft.com** .
    
    *Dica: Você também pode usar o favorito do Serviço do Power BI na barra de favoritos do Microsoft Edge.*
    
3. Clique **em Entrar** (localizado no canto superior direito).
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image2.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image2.png)
    
4. Conclua o processo de login.
5. Se solicitado pelo Microsoft Edge para permanecer conectado, clique em **Sim** .
6. Na janela do navegador Microsoft Edge, no serviço Power BI, no painel **Navegação** , expanda **Meu Workspace** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image3.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image3.png)
    
7. Deixe a janela do navegador Microsoft Edge aberta.

### Tarefa 2: Começar – Abrir relatório

Nesta tarefa, você configurará o ambiente do laboratório abrindo o relatório inicial.

*Importante: Se você continua no laboratório anterior (e concluiu esse laboratório com êxito), não conclua esta tarefa; em vez disso, continue a partir da próxima tarefa.*

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image4.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image4.png)
    
2. Para fechar a janela de introdução, no canto superior esquerdo da janela, clique em **X** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image5.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image5.png)
    
3. Para entrar no serviço do Power BI, no canto superior direito, clique em **Entrar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image6.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image6.png)
    
4. Conclua o processo de entrada usando a mesma conta usada para entrar no serviço do Power BI.
5. Para abrir o arquivo inicial do Power BI Desktop, clique na guia da faixa de opções **Arquivo** para abrir o modo de exibição de bastidores.
6. Selecione **Abrir relatório** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image7.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image7.png)
    
7. Clique **em Procurar relatórios** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image8.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image8.png)
    
8. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\07-design-report-in-power-bi-desktop-enhanced\Starter** .
9. Selecione o arquivo de **Análise de Vendas** .
10. Clique **em Abrir** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image9.png)
    
11. Feche todas as janelas informativas que possam ser abertas.
12. Para criar uma cópia do arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
13. Selecione **Salvar como** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image10.png)
    
14. Se solicitado a aplicar as alterações, clique em **Aplicar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image11.png)
    
15. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
16. Clique **em Salvar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image12.png)
    

### **Tarefa 3: sincronize segmentações**

Nesta tarefa, você sincronizará as segmentações de **ano** e **região .**

*Você continuará o desenvolvimento do relatório criado no laboratório **Criar um Relatório no Power BI Desktop, Parte 1 .***

1. No Power BI Desktop, na página **Visão geral** , defina a segmentação de dados **Year** como **FY2018** .
2. Vá para a página **Meu desempenho** e observe que a segmentação de **ano** é um valor diferente.
    
    *Quando as segmentações não são sincronizadas, isso pode contribuir para a deturpação dos dados e para a frustração dos usuários de relatórios. Agora você sincronizará as segmentações de relatórios.*
    
3. Retorne à página **Visão geral** e selecione a segmentação de **ano** .
4. Na guia **Exibir** faixa de opções, de dentro do grupo **Mostrar painéis** , clique em **Sincronizar fatiadores** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image13.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image13.png)
    
5. No painel **Sync Slicers** (à esquerda do painel **Visualizações** ), na segunda coluna (que representa a sincronização), marque as caixas de seleção das páginas **Visão geral** e **Meu desempenho .**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image14.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image14.png)
    
6. Na página **Visão geral** , selecione a segmentação de **região** .
7. Sincronize a segmentação de dados com as páginas **Visão geral** e **Lucro .**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image15.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image15.png)
    
8. Teste as segmentações sincronizadas selecionando diferentes opções de filtro e, em seguida, verificando se as segmentações sincronizadas filtram pela mesma seleção.
9. Para fechar a página do **Sync Slicer** , clique no **X** localizado no canto superior direito do painel.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image16.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image16.png)
    

## **Exercício 2: Configurar Drill Through**

Neste exercício, você criará uma nova página e a configurará como uma página de drill through. Quando você tiver concluído o design, a página terá a seguinte aparência:

![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image17.png)

### **Tarefa 1: criar uma página de detalhamento**

Nesta tarefa, você criará uma nova página e a configurará como uma página de drill through.

1. Adicione uma nova página de relatório chamada **Detalhes do produto** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image18.png)
    
2. Clique com o botão direito do mouse na guia da página **Detalhes do produto** e selecione **Ocultar página** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image19.png)
    
    *Os usuários do relatório não poderão acessar a página de detalhamento diretamente. Eles precisarão acessá-lo a partir de recursos visuais em outras páginas. Você aprenderá a detalhar a página no exercício final deste laboratório.*
    
3. Abaixo do painel **Visualizações , na seção Drill Through** , adicione o **Product |** Campo de **categoria para a caixa Adicionar campos de drill-through aqui** .
    
    *Os laboratórios usam uma notação abreviada para fazer referência a um campo. Ficará assim: **Produto | Categoria** . Neste exemplo, **Product** é o nome da tabela e **Category** é o nome do campo.*
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image20.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image20.png)
    
4. Para testar a página de detalhamento, no cartão de filtro de detalhamento, selecione **Bicicletas** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image21.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image21.png)
    
5. No canto superior esquerdo da página do relatório, observe o botão de seta.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image22.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image22.png)
    
    *Um botão é adicionado automaticamente quando um campo é adicionado ao poço/área de perfuração. Ele permite que os usuários do relatório naveguem de volta para a página da qual fizeram o drill through.*
    
6. Adicione um visual de **cartão** à página e, em seguida, redimensione e posicione-o para que fique à direita do botão e preencha a largura restante da página.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image23.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image23.png)
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image24.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image24.png)
    
7. Arraste o **Produto | Campo de categoria** no visual do cartão.
8. Configure as opções de formato para o visual e, em seguida, desative a propriedade **Category Label** para **Off** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image36b.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image36b.png)
    
9. Defina a propriedade **Efeitos >** Cor de fundo para um tom claro de cinza.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image36c.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/07-design-report-in-power-bi-desktop_image36c.png)
    
10. Adicione um visual de **Tabela** à página e, em seguida, redimensione-o e posicione-o para que fique abaixo do visual do cartão e preencha o espaço restante na página.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image26.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image26.png)
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image27.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image27.png)
    
11. Adicione os seguintes campos ao visual:
    - Produto | Subcategoria
    - Produto | Cor
    - Vendas | Quantidade
    - Vendas | Vendas
    - Vendas | Margem de lucro
12. Configure as opções de formato para o visual e, na seção **Valores** , defina a propriedade **Tamanho do Texto como 20pt** .
    
    *O design da página de drill through está quase completo. Você aprimorará a página com formatação condicional no próximo exercício.*
    

## **Exercício 3: Adicionar formatação condicional**

Neste exercício, você aprimorará a página de drill through com formatação condicional. Quando você tiver concluído o design, a página terá a seguinte aparência:

![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image28.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image28.png)

### **Tarefa 1: adicionar formatação condicional**

Nesta tarefa, você aprimorará a página de drill through com formatação condicional.

1. Selecione o visual da tabela.
2. No painel de visualização, clique na seta para baixo no valor da **Margem de Lucro** e selecione **Formatação Condicional | Ícones** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image29.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image29.png)
    
3. Na janela **Ícones – Margem de lucro , na lista suspensa Layout do ícone** , selecione **Direito dos dados** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image30.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image30.png)
    
4. Para excluir a régua do meio, à esquerda do triângulo amarelo, clique em **X** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image31.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image31.png)
    
5. Configure a primeira regra (losango vermelho) da seguinte forma:
    - No segundo controle, remova o valor
    - No terceiro controle, selecione **Número**
    - No quinto controle, digite **0**
    - No sexto controle, selecione **Número**
6. Configure a segunda regra (círculo verde) da seguinte forma:
    - No segundo controle, digite **0**
    - No terceiro controle, selecione **Número**
    - No quinto controle, remova o valor
    - No sexto controle, selecione **Número**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image32.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image32.png)
    
    *As regras podem ser interpretadas da seguinte forma: exibir um losango vermelho se o valor da margem de lucro for menor que 0; caso contrário, se o valor for grande ou igual a zero, exiba um círculo verde.*
    
7. Clique **em OK** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image33.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image33.png)
    
8. No visual da tabela, verifique se os ícones corretos são exibidos.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image34.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image34.png)
    
9. Configure a formatação condicional da cor de fundo para o campo **Cor** .
10. Na janela Cor de **fundo – Cor** , na lista suspensa **Estilo de formato** , selecione **Valor do campo** .
11. No **campo em que devemos basear isso?** lista suspensa, selecione **Produto | Formatação | Formato de cor de fundo** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image36.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image36.png)
    
12. Clique **em OK** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image37.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image37.png)
    
13. Repita as etapas anteriores para configurar a formatação condicional da cor da fonte para o campo **Cor** , usando o **Produto | Formatação |** Campo de **formato de cor da fonte**
    
    *Você deve se lembrar de que as cores do plano de fundo e da fonte foram originadas do arquivo **ColorFormats.csv no laboratório Preparar Dados no Power BI Desktop** e, em seguida, integradas à consulta do **Produto no laboratório Carregar Dados no Power BI Desktop** .*
    

## **Exercício 4: Adicionar marcadores e botões**

Neste exercício, você aprimorará a página **Meu desempenho** com botões, permitindo que o usuário do relatório selecione o tipo de visual a ser exibido. Quando você tiver concluído o design, a página terá a seguinte aparência:

![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image38.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image38.png)

### **Tarefa 1: adicionar marcadores**

Nesta tarefa, você adicionará dois marcadores, um para exibir cada um dos visuais mensais de vendas/alvos.

1. Vá para a página **Meu desempenho** .
2. Na guia **Exibir** faixa de opções, de dentro do grupo **Mostrar Painéis** , clique em **Marcadores** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image39.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image39.png)
    
3. Na guia **Exibir** faixa de opções, de dentro do grupo **Mostrar painéis** , clique em **Seleção** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image40.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image40.png)
    
4. No painel **Seleção , ao lado de um dos itens Vendas e Meta por mês** , para ocultar o visual, clique no ícone de olho.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image41.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image41.png)
    
5. No painel **Marcadores** , clique em **Adicionar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image42.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image42.png)
    
6. Para renomear o marcador, clique duas vezes no marcador.
7. Se o gráfico visível for o gráfico de barras, renomeie o marcador como **Gráfico de Barras ON** , caso contrário renomeie o marcador como **Gráfico de Colunas ON** .
8. Para editar o marcador, no painel **Marcadores** , passe o cursor sobre o marcador, clique nas reticências e selecione **Dados** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image43.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image43.png)
    
    *Desabilitar a opção **Dados** significa que o marcador não usará o estado atual do filtro. Isso é importante porque, caso contrário, o marcador bloquearia permanentemente o filtro aplicado atualmente pela segmentação de **ano** .*
    
9. Para atualizar o marcador, clique nas reticências novamente e selecione **Atualizar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image44.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image44.png)
    
    *Nas etapas a seguir, você criará e configurará um segundo marcador para mostrar o segundo visual.*
    
10. No painel **Seleção** , alterne a visibilidade dos dois itens **Vendas e Meta por mês** .
    
    *Em outras palavras, torne o visual visível oculto e torne o visual oculto visível.*
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image45.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image45.png)
    
11. Crie um segundo marcador e nomeie-o adequadamente ( Gráfico de **Colunas ATIVADO** ou **Gráfico de Barras ATIVADO).**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image46.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image46.png)
    
12. Configure o segundo marcador para ignorar os filtros ( opção de **dados** desativada) e atualize o marcador.
13. No painel **Seleção** , para tornar os dois visuais visíveis, basta mostrar o visual oculto.
14. Redimensione e reposicione os dois visuais para que eles preencham a página abaixo do visual de vários cartões e se sobreponham completamente.
    
    *Dica: Para selecionar o visual que está encoberto, selecione-o no painel **Seleção .***
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image47.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image47.png)
    
15. No painel **Marcadores** , selecione cada um dos marcadores e observe que apenas um dos visuais está visível.
    
    *A próxima etapa do design é adicionar dois botões à página, o que permitirá que o usuário do relatório selecione os marcadores.*
    

### **Tarefa 2: Adicionar botões**

Nesta tarefa, você adicionará dois botões e atribuirá ações de favoritos a cada um.

1. Na faixa de opções **Inserir , de dentro do grupo Elementos** , clique em **Botão** e selecione Em **branco** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image48.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image48.png)
    
2. Posicione o botão diretamente abaixo da segmentação de **ano** .
3. Selecione o botão e, no painel de **botões Formatar , clique em Geral** e ative a propriedade **Título para Ativado** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image49b.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image49b.png)
    
4. Expanda a seção **Título e, na caixa Texto** , insira **Gráfico de barras** .
5. Expanda a seção Plano de **fundo** e defina uma cor de plano de fundo usando uma cor complementar.
6. Clique em **Button** e ative a propriedade **Action para On** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image50.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image50.png)
    
7. Expanda a seção **Ação** e defina a lista suspensa **Tipo como Marcador** .
8. Na lista suspensa **Marcador** , selecione **Gráfico de barras ATIVADO** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image51.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image51.png)
    
9. Crie uma cópia do botão usando copiar e colar e configure o novo botão da seguinte maneira:
    
    *Dica: Os comandos de atalho para copiar e colar são **Ctrl+C** seguidos de **Ctrl+V** .*
    
    - Defina a propriedade **Texto do botão como Gráfico de colunas**
    - Na seção **Ação** , defina a lista suspensa **Marcador como Gráfico de colunas ATIVADO**
    
    *O design do relatório de Análise de Vendas agora está completo.*
    

### **Tarefa 3: publique o relatório**

Nesta tarefa você publicará o relatório.

1. Selecione a página **Visão geral** .
2. Na segmentação de **ano** , selecione **FY2020** .
3. Na segmentação de **região** , selecione **Selecionar tudo** .
4. Salve o arquivo do Power BI Desktop.
    
    *O arquivo sempre deve ser salvo antes da publicação no serviço do Power BI.*
    
5. Na guia da faixa de opções **Home , de dentro do grupo Compartilhar** , clique em **Publicar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image52.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image52.png)
    
6. Na janela **Publicar no Power** BI, observe que **Meu Workspace** está selecionado.
7. Para publicar o relatório, clique em **Selecionar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image53.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image53.png)
    
8. Se solicitado a substituir o conjunto de dados, clique em **Substituir** .
9. Quando a publicação for bem-sucedida, clique em **Entendi** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image54.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image54.png)
    
10. Feche o Power BI Desktop.
    
    *Você explorará o relatório no serviço do Power BI no próximo exercício.*
    

## **Exercício 5: Explore o Relatório**

Neste exercício, você explorará o relatório no serviço do Power BI.

### **Tarefa 1: explore o relatório**

Nesta tarefa, você explorará o relatório no serviço do Power BI.

1. Na janela do navegador Microsoft Edge, no serviço Power BI, no painel **Navegação** , selecione **Meu Workspace** e clique no relatório **Análise de Vendas .**
2. Para testar o relatório de drill through, na página **Visão geral** , no visual **Quantidade por Categoria , clique com o botão direito do mouse na barra Vestuário** e selecione **Drill Through | Detalhes do produto** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image55.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image55.png)
    
3. Observe que a página de **detalhes do produto** é para **vestuário** .
4. Para retornar à página de origem, no canto superior esquerdo da página, clique no botão de seta.
5. Selecione a página **Meu desempenho** .
6. Clique em cada um dos botões e observe que um visual diferente é exibido.

### **Tarefa 2: Concluir**

Nesta tarefa, você concluirá o laboratório.

1. Para retornar ao seu espaço de trabalho, no banner da página da Web da janela, clique em **Meu Espaço** de Trabalho .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image56.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/08-design-report-in-power-bi-desktop-enhanced_image56.png)
    
2. Deixe a janela do navegador Microsoft Edge aberta.

# Parabéns!