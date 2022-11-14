# **Instruções de laboratório**

# **Analise dados com visuais de IA**

**O tempo estimado para concluir o laboratório é de 45 minutos**

Neste laboratório, você criará o relatório **Sales Exploration** .

Neste laboratório, você aprenderá a:

- Crie gráficos de dispersão animados
- Use um visual para prever valores

### **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. Preparar dados no Power BI Desktop
2. Carregar dados no Power BI Desktop
3. Dados do modelo no Power BI Desktop
4. Criar cálculos DAX no Power BI Desktop, Parte 1
5. Criar cálculos DAX no Power BI Desktop, Parte 2
6. Projetar um relatório no Power BI Desktop, Parte 1
7. Projetar um relatório no Power BI Desktop, Parte 2
8. **Analise dados com visuais de IA**
9. Criar um painel do Power BI
10. Aplicar segurança em nível de linha

## **Exercício 1: Criar o Relatório**

Neste exercício, você criará o relatório **Exploração de vendas .**

### **Tarefa 1: Começar – Entrar**

Nesta tarefa, você configurará o ambiente do laboratório entrando no Power BI.

*Importante: Se você já entrou no Power BI em um laboratório anterior, continue na próxima tarefa.*

1. Para abrir o Microsoft Edge, na barra de tarefas, clique no atalho do programa Microsoft Edge.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image1.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image1.png)
    
2. Na janela do navegador Microsoft Edge, navegue até **https://powerbi.microsoft.com** .
    
    *Dica: Você também pode usar o favorito do Serviço do Power BI na barra de favoritos do Microsoft Edge.*
    
3. Clique **em Entrar** (localizado no canto superior direito).
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image2.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image2.png)
    
4. Insira os detalhes da conta fornecidos a você.
5. Se solicitado a atualizar a senha, digite novamente a senha fornecida e, em seguida, digite e confirme uma nova senha.
    
    *Importante: Certifique-se de registrar sua nova senha.*
    
6. Conclua o processo de login.
7. Se solicitado pelo Microsoft Edge para permanecer conectado, clique em **Sim** .
8. Na janela do navegador Microsoft Edge, no serviço Power BI, no painel **Navegação** , expanda **Meu Workspace** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image3.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image3.png)
    
9. Deixe a janela do navegador Microsoft Edge aberta.

### **Tarefa 2: Começar – Criar um conjunto de dados**

Nesta tarefa, você configurará o ambiente do laboratório criando um conjunto de dados.

*Importante: Se você já publicou o conjunto de dados no laboratório **Criar um painel do Power BI** , continue na próxima tarefa.*

1. Na janela do navegador Microsoft Edge, no serviço Power BI, no painel **Navegação , na parte inferior, clique em Obter Dados** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image4.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image4.png)
    
2. No bloco **Arquivos** , clique em **Obter** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image5.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image5.png)
    
3. Clique no bloco **Arquivo local .**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image6.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image6.png)
    
4. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\08-create-power-bi-dashboard\Solution** .
5. Selecione o arquivo **Sales Analysis.pbix** e clique em **Abrir** .
6. Se solicitado a substituir o conjunto de dados, clique em **Substituir** .

### **Tarefa 3: crie o relatório**

Nesta tarefa, você criará o relatório **Exploração de vendas .**

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.
    
    *Importante: Se você já tiver o Power BI Desktop aberto (de um laboratório anterior), feche essa instância.*
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image7.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image7.png)
    
2. Para fechar a janela de introdução, no canto superior esquerdo da janela, clique em **X** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image8.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image8.png)
    
3. Se o Power BI Desktop não estiver conectado ao serviço do Power BI, no canto superior direito, clique em **Entrar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image9.png)
    
4. Conclua o processo de entrada usando a mesma conta usada para entrar no serviço do Power BI.
5. Para salvar o arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
6. Selecione **Salvar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image10.png)
    
7. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
8. Na caixa **Nome do arquivo** , insira **Exploração de vendas** e clique em **Salvar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image11.png)
    
9. Para criar uma conexão em tempo real com o conjunto de dados de **Análise de Vendas** , na guia da faixa de opções **Home , de dentro do grupo Dados** , clique em **Conjuntos de Dados do Power BI** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image12.png)
    
10. Na janela **Selecionar um conjunto de dados para criar um relatório , selecione o conjunto de dados Análise de vendas** .
11. Clique **em Criar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image13.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image13.png)
    
12. Salve o arquivo do Power BI Desktop.
    
    *Agora você criará duas páginas de relatório e, em cada página, trabalhará com um visual diferente para analisar e explorar dados.*
    

## **Exercício 2: Crie um gráfico de dispersão**

Neste exercício, você criará um gráfico de dispersão que pode ser animado.

### **Tarefa 1: crie um gráfico de dispersão animado**

Nesta tarefa, você criará um gráfico de dispersão que pode ser animado.

1. Renomeie a **página 1** como **gráfico de dispersão** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image14.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image14.png)
    
2. Adicione um visual de **gráfico de dispersão** à página do relatório e, em seguida, posicione e redimensione-o para que preencha a página inteira.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image15.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image15.png)
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image16.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image16.png)
    
3. Adicione os seguintes campos aos poços/áreas visuais:
    
    Os laboratórios usam uma notação abreviada para fazer referência a um campo. Ficará assim: **Revendedor | Tipo de negócio** . Neste exemplo, **Revendedor** é o nome da tabela e **Tipo de Negócio** é o nome do campo.
    
    - Eixo X: **Vendas | Vendas**
    - Eixo Y: **Vendas | Margem de lucro**
    - Legenda: **Revendedor | Tipo de Negócio**
    - Tamanho: **Vendas | Quantidade**
    - Eixo de Reprodução: **Data | Trimestre**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image17.png)
    
    *O gráfico pode ser animado quando um campo é adicionado ao poço/área do **Eixo de Reprodução .***
    
4. No painel **Filtros , adicione o Produto | Campo Categoria** para o poço/área **Filtros nesta página .**
5. No cartão de filtro, filtre por **Bicicletas** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image18.png)
    
6. Para animar o gráfico, no canto inferior esquerdo, clique em **Reproduzir** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image19.png)
    
7. Assista a todo o ciclo de animação do **primeiro trimestre** do ano fiscal de 2018 ao **quarto trimestre** do ano fiscal de 2020 .
    
    *O gráfico de dispersão permite entender os valores da medida simultaneamente: neste caso, quantidade do pedido, receita de vendas e margem de lucro.*
    
    *Cada bolha representa um tipo de negócio de revendedor. As alterações no tamanho da bolha refletem quantidades de pedidos aumentadas ou diminuídas. Enquanto os movimentos horizontais representam aumentos/diminuições na receita de vendas e os movimentos verticais representam aumentos/diminuições na lucratividade.*
    
8. Quando a animação parar, clique em uma das bolhas para revelar seu rastreamento ao longo do tempo.
9. Passe o cursor sobre qualquer bolha para revelar uma dica de ferramenta descrevendo os valores de medida para o tipo de revendedor naquele momento.
10. No painel **Filtros , filtre apenas por Roupas** e observe que isso produz um resultado muito diferente.
11. Salve o arquivo do Power BI Desktop.

## **Exercício 3: Criar uma previsão**

Neste exercício, você criará uma previsão para determinar possíveis receitas de vendas futuras.

### **Tarefa 1: crie uma previsão**

Nesta tarefa, você criará uma previsão para determinar possíveis receitas de vendas futuras.

1. Adicione uma nova página e renomeie a página para **Previsão** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image20.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image20.png)
    
2. Adicione um visual de **gráfico de linhas** à página do relatório e, em seguida, posicione e redimensione-o para que preencha a página inteira.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image21.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image21.png)
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image22.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image22.png)
    
3. Adicione os seguintes campos aos poços/áreas visuais:
    - Eixo X: **Data | Encontro**
    - Eixo Y: **Vendas | Vendas**
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image23.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image23.png)
    
4. No painel **Filtros , adicione a Data |** campo **Ano** para o poço/área **Filtros nesta página .**
5. No cartão de filtro, filtre por dois anos: **FY2019** e **FY2020** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image24.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image24.png)
    
    *Ao prever em uma linha do tempo, você precisará de pelo menos dois ciclos (anos) de dados para produzir uma previsão precisa e estável.*
    
6. Adicione também o **Produto | Categoria** para o poço/área **Filtros nesta página** e filtre por **Bicicletas** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image25.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image25.png)
    
7. Para adicionar uma previsão, abaixo do painel **Visualizações** , selecione o painel **Analytics** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image26.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image26.png)
    
8. Expanda a seção **Previsão** .
    
    *Se a seção **Previsão** não estiver disponível, provavelmente é porque o visual não foi configurado corretamente. A previsão só está disponível quando duas condições são atendidas: o eixo tem um único campo do tipo data e há apenas um campo de valor.*
    
9. Ative **a** opção **Previsão** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image28.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image28.png)
    
10. Configure as seguintes propriedades de previsão:
    - Unidades: Meses
    - Duração da previsão: 1 mês
    - Sazonalidade: 365
    - Intervalo de confiança: 80%
11. Clique **em Aplicar** .
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image29.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image29.png)
    
12. No visual de linha, observe que a previsão se estendeu um mês além dos dados do histórico.
    
    *A área cinza representa a confiança. Quanto maior a confiança, menos estável - e, portanto, menos precisa - a previsão provavelmente será.*
    
    *Quando souber a duração do ciclo, neste caso anual, deverá introduzir os pontos de sazonalidade. Às vezes, pode ser semanal (7) ou mensal (30).*
    
13. No painel **Filtros , filtre apenas por Roupas** e observe que isso produz um resultado diferente.
14. Salve o arquivo do Power BI Desktop.

### **Tarefa 2: Concluir**

Nesta tarefa, você concluirá o laboratório.

1. Selecione a página **Gráfico de Dispersão** .
2. Salve o arquivo do Power BI Desktop.
3. Para publicar o arquivo em seu **espaço** de trabalho , na guia da faixa de opções **Home , de dentro do grupo Compartilhar** , clique em **Publicar** e, em seguida, clique em **Selecionar** para publicar.
    
    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image46.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/10-perform-data-analysis-in-power-bi-desktop_image46.png)
    
4. Feche o Power BI Desktop.

# Parabéns!