# **Instruções de laboratório**

# Projetar um modelo de dados no Power BI

**O tempo estimado para concluir o laboratório é de 45 minutos.**

Neste laboratório, você começará a desenvolver o modelo de dados. Isso envolverá a criação de relacionamentos entre tabelas e, em seguida, a configuração de propriedades de tabela e coluna para melhorar a facilidade e usabilidade do modelo de dados. Você também criará hierarquias e criará medidas rápidas.

Neste laboratório, você aprenderá a:

- Criar relacionamentos de modelo
- Configurar propriedades de tabela e coluna
- Criar hierarquias

### **História do laboratório**

Este laboratório é um dos muitos de uma série de laboratórios que foram projetados como uma história completa, desde a preparação de dados até a publicação como relatórios e painéis. Você pode concluir os laboratórios em qualquer ordem. No entanto, se você pretende trabalhar em vários laboratórios, sugerimos que você os faça na seguinte ordem:

1. Preparar dados no Power BI Desktop
2. Carregar dados no Power BI Desktop
3. **Projetar um modelo de dados no Power BI**
4. Criar cálculos DAX no Power BI Desktop, Parte 1
5. Criar cálculos DAX no Power BI Desktop, Parte 2
6. Projetar um relatório no Power BI Desktop, Parte 1
7. Projetar um relatório no Power BI Desktop, Parte 2
8. Analise dados com visuais de IA
9. Criar um painel do Power BI
10. Aplicar segurança em nível de linha

## **Exercício 1: Criar Relacionamentos Modelo**

Neste exercício, você criará relacionamentos de modelo.

### **Tarefa 1: comece**

Nesta tarefa, você configurará o ambiente para o laboratório.

_Importante: Se você continua no laboratório anterior (e concluiu esse laboratório com êxito), não conclua esta tarefa; em vez disso, continue a partir da próxima tarefa._

1. Para abrir o Power BI Desktop, na barra de tarefas, clique no atalho do Microsoft Power BI Desktop.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image1.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image1.png)

2. Para fechar a janela de introdução, no canto superior esquerdo da janela, clique em **X** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image2.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image2.png)

3. Para abrir o arquivo inicial do Power BI Desktop, clique na guia da faixa de opções **Arquivo** para abrir o modo de exibição de bastidores.
4. Selecione **Abrir relatório** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image3.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image3.png)

5. Clique **em Procurar relatórios** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image4.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image4.png)

6. Na janela **Abrir , navegue até a pasta D:\PL300\Labs\03-configure-data-model-in-power-bi-desktop\Starter** .
7. Selecione o arquivo de **Análise de Vendas** .
8. Clique **em Abrir** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image5.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image5.png)

9. Feche todas as janelas informativas que possam ser abertas.
10. Para criar uma cópia do arquivo, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
11. Selecione **Salvar como** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image6.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image6.png)

12. Se solicitado a aplicar as alterações, clique em **Aplicar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image7.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image7.png)

13. Na janela **Salvar como , navegue até a pasta D:\PL300\MySolution** .
14. Clique **em Salvar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image8.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image8.png)

### **Tarefa 2: criar relacionamentos de modelo**

Nesta tarefa, você criará relacionamentos de modelo.

1. No Power BI Desktop, à esquerda, clique no ícone Exibição do **modelo .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image9.png)

2. Se você não vir todas as sete tabelas, role horizontalmente para a direita e, em seguida, arraste e organize as tabelas mais próximas para que possam ser vistas ao mesmo tempo.

   _Dica: Você também pode usar o controle de zoom localizado na parte inferior da janela._

   _Na visualização Modelo, é possível visualizar cada tabela e relacionamentos (conectores entre tabelas). Atualmente, não há relacionamentos porque no laboratório **Preparar Dados no Power BI Desktop** , você desativou as opções de relacionamento de carregamento de dados._

3. Para retornar à visualização Relatório, à esquerda, clique no ícone Visualização **Relatório .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image10.png)

4. Para exibir todos os campos da tabela, no painel **Campos** , clique com o botão direito do mouse em uma área vazia e selecione **Expandir tudo** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image11.png)

5. Para criar um visual de tabela, no painel **Campos , de dentro da tabela Produto** , verifique o campo **Categoria** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image12.png)

   _Os laboratórios usam uma notação abreviada para fazer referência a um campo. Ficará assim: **Produto | Categoria** . Neste exemplo, **Product** é o nome da tabela e **Category** é o nome do campo._

6. Para adicionar uma coluna adicional à tabela, no painel **Campos , marque a caixa Vendas | Campo de vendas** .
7. Observe que o visual da tabela lista quatro categorias de produtos e que o valor de vendas é o mesmo para cada uma e o mesmo para o total.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image13.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image13.png)

   _O problema é que a tabela é baseada em campos de tabelas diferentes. A expectativa é que cada categoria de produto exiba as vendas dessa categoria. No entanto, como não há um relacionamento de modelo entre essas tabelas, a tabela **Sales** não é filtrada. Agora você adicionará um relacionamento para propagar filtros entre as tabelas._

8. Na guia **Modelagem , no grupo Relacionamentos** , clique em **Gerenciar Relacionamentos** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image14.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image14.png)

9. Na janela **Gerenciar Relacionamentos** , observe que nenhum relacionamento ainda está definido.
10. Para criar um relacionamento, clique em **Novo** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image15.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image15.png)

11. Na janela **Criar Relacionamento** , na primeira lista suspensa, selecione a tabela **Produto .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image16.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image16.png)

12. Na segunda lista suspensa (abaixo da grade da tabela **Produto** ), selecione a tabela **Vendas .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image17.png)

13. Observe que as colunas **ProductKey** em cada tabela foram selecionadas automaticamente.

    _As colunas foram selecionadas porque compartilham o mesmo nome e tipo de dados._

14. Na lista suspensa **Cardinalidade** , observe que **Um para muitos (1:\*)** está selecionado.

    _A cardinalidade foi detectada automaticamente porque o Power BI entende que a coluna **ProductKey da tabela Product** contém valores exclusivos. Os relacionamentos um-para-muitos são a cardinalidade mais comum, e todos os relacionamentos que você criar neste laboratório serão desse tipo._

15. Na lista suspensa **Cross Filter Direction** , observe que **Single** está selecionado.

    _Direção de filtro único significa que os filtros se propagam de “um lado” para “muitos lados”. Nesse caso, significa que os filtros aplicados à tabela **Product** serão propagados para a tabela **Sales** , mas não na direção oposta._

16. Observe que **Mark This Relationship Active** está marcado.

    _Relacionamentos ativos propagam filtros. É possível marcar um relacionamento como inativo para que os filtros não se propaguem. Relacionamentos inativos podem existir quando há vários caminhos de relacionamento entre tabelas. Nesse caso, os cálculos do modelo podem usar funções especiais para ativá-los._

17. Clique **em OK** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image18.png)

18. Na janela **Gerenciar Relacionamentos** , observe que o novo relacionamento está listado e clique em **Fechar** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image19.png)

19. No relatório, observe que o visual da tabela foi atualizado para exibir valores diferentes para cada categoria de produto.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image20.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image20.png)

    _Os filtros aplicados à tabela **Product** agora se propagam para a tabela **Sales** ._

20. Alterne para o modo de exibição de modelo e observe que agora há um conector entre as duas tabelas (não importa se as tabelas estão posicionadas uma ao lado da outra).

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image21.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image21.png)

21. No diagrama, observe que você pode interpretar a cardinalidade representada pelos indicadores **1** e \*\*\*\* .

    _A direção do filtro é representada pela ponta da seta. Uma linha sólida representa um relacionamento ativo; uma linha tracejada representa um relacionamento inativo._

22. Passe o cursor sobre o relacionamento para destacar as colunas relacionadas.

    _Há uma maneira mais fácil de criar um relacionamento. No diagrama de modelo, você pode arrastar e soltar colunas para criar um novo relacionamento._

23. Para criar um novo relacionamento usando uma técnica diferente, na tabela **Reseller , arraste a coluna ResellerKey** para a coluna **ResellerKey** da tabela **Sales .**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image22.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image22.png)

    _Dica: Às vezes, uma coluna não quer ser arrastada. Se essa situação ocorrer, selecione uma coluna diferente e, em seguida, selecione a coluna que você pretende arrastar novamente e tente novamente. Certifique-se de ver o novo relacionamento adicionado ao diagrama._

24. Use a nova técnica para criar os dois relacionamentos de modelo a seguir:
    - **Região | SalesTerritoryKey** to **Sales | Chave de território de vendas**
    - **Vendedor | EmployeeKey** to **Sales | EmployeeKey**
25. No diagrama, organize as tabelas de forma que a tabela **Vendas** seja posicionada no centro do diagrama e as tabelas relacionadas sejam organizadas sobre ela. Posicione as mesas desconectadas ao lado.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image23.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image23.png)

26. Salve o arquivo do Power BI Desktop.

## **Exercício 2: Configurar Tabelas**

Neste exercício, você configurará cada tabela criando hierarquias e ocultando, formatando e categorizando colunas.

### **Tarefa 1: configurar a tabela de produtos**

Nesta tarefa você irá configurar a tabela **Produto .**

1. Na visualização Modelo, no painel **Campos** , se necessário, expanda a tabela **Produto** para revelar todos os campos.
2. Para criar uma hierarquia, no painel **Campos , clique com o botão direito do mouse na coluna Categoria** e selecione **Criar hierarquia** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image24.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image24.png)

3. No painel **Propriedades** (à esquerda do painel **Campos** ), na caixa **Nome** , substitua o texto por **Produtos** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image25.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image25.png)

4. Para adicionar o segundo nível à hierarquia, no painel **Propriedades , na lista suspensa Hierarquia** , selecione **Subcategoria** (talvez seja necessário rolar para baixo dentro do painel).
5. Para adicionar o terceiro nível à hierarquia, na lista suspensa **Hierarquia** , selecione **Produto** .
6. Para concluir o design da hierarquia, clique em **Aplicar alterações de nível** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image26.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image26.png)

   _Dica: Não se esqueça de clicar em **Aplicar alterações de nível** — é um erro comum ignorar esta etapa._

7. No painel **Campos** , observe a hierarquia de **Produtos .**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image27.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image27.png)

8. Para revelar os níveis de hierarquia, expanda a hierarquia **Produtos** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image28.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image28.png)

9. Para organizar colunas em uma pasta de exibição, no painel **Campos** , primeiro selecione a coluna **Formato de cor de fundo .**
10. Enquanto pressiona a tecla **Ctrl** , selecione a coluna **Font Color Format .**
11. No painel **Propriedades , na caixa Pasta de exibição** , insira **Formatação** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image29.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image29.png)

12. No painel **Campos** , observe que as duas colunas agora estão dentro de uma pasta.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image30.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image30.png)

    _As pastas de exibição são uma ótima maneira de organizar as tabelas, especialmente para as tabelas que incluem muitos campos._

### **Tarefa 2: configurar a tabela de regiões**

Nesta tarefa você irá configurar a tabela **Region .**

1. Na tabela **Region** , crie uma hierarquia chamada **Regions** , com os três níveis a seguir:

   - Grupo
   - País
   - Região

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image31.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image31.png)

2. Selecione a coluna **País** (não o nível de hierarquia **País ).**
3. No painel **Propriedades** , expanda a seção **Avançado** (na parte inferior do painel) e, na lista suspensa **Categoria de dados** , selecione **País/Região** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image32.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image32.png)

   _A categorização de dados pode fornecer dicas para o designer de relatórios. Nesse caso, categorizar a coluna como país ou região fornece informações mais precisas ao Power BI ao renderizar uma visualização de mapa._

### **Tarefa 3: configurar a tabela de revendedores**

Nesta tarefa você irá configurar a tabela **Revendedor .**

1. Na tabela **Revendedor** , crie uma hierarquia chamada **Revendedores** , com os dois níveis a seguir:

   - Tipo de Negócio
   - Revendedor

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image33.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image33.png)

2. Crie uma segunda hierarquia chamada **Geografia** , com os quatro níveis a seguir:

   - País-Região
   - Estado-Província
   - Cidade
   - Revendedor

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image34.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image34.png)

3. Defina a **categoria de dados** para as colunas **Country-Region** , **State-Province** e **City** (não o nível de hierarquia) como **Country/Region** , **State ou Province** e **City** , respectivamente.

### **Tarefa 4: configurar a tabela Sales**

Nesta tarefa você irá configurar a tabela **Sales .**

1. Na tabela **Vendas** , selecione a coluna **Custo .**
2. No painel **Propriedades , na caixa Descrição** , insira: **Com base no custo padrão**

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image35.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image35.png)

   _As descrições podem ser aplicadas a tabelas, colunas, hierarquias ou medidas. No painel **Campos** , o texto da descrição é revelado em uma dica de ferramenta quando um autor de relatório passa o cursor sobre o campo._

3. Selecione a coluna **Quantidade .**
4. No painel **Propriedades , na seção Formatação** , deslize a propriedade **Separador de milhares para Sim** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image36.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image36.png)

5. Selecione a coluna **Preço unitário .**
6. No painel **Propriedades , na seção Formatação** , defina a propriedade Casas **decimais como 2** .
7. No grupo **Avançado** (talvez seja necessário rolar para baixo para localizá-lo), na lista suspensa **Resumir por , selecione Média** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image37.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image37.png)

   _Por padrão, as colunas numéricas serão resumidas somando os valores. Esse comportamento padrão não é adequado para uma coluna como **Unit Price** , que representa uma taxa. Definir a sumarização padrão como média produzirá um resultado significativo._

### **Tarefa 5: propriedades de atualização em massa**

Nesta tarefa, você atualizará várias colunas usando atualizações em massa únicas. Você usará essa abordagem para ocultar colunas e formatar valores de coluna.

1. No painel **Campos , selecione o Produto | coluna ProductKey** .
2. Enquanto pressiona a tecla **Ctrl** , selecione as 13 colunas a seguir (abrangendo várias tabelas):
   - Região | Chave de território de vendas
   - Revendedor | Chave do revendedor
   - Vendas | EmployeeKey
   - Vendas | Chave do produto
   - Vendas | Chave do revendedor
   - Vendas | Número do pedido de vendas
   - Vendas | Chave de território de vendas
   - Vendedor | ID do Empregado
   - Vendedor | EmployeeKey
   - Vendedor | UPN
   - VendedorRegião | EmployeeKey
   - VendedorRegião | Chave de território de vendas
   - Alvos | ID do Empregado
3. No painel **Propriedades , deslize a propriedade Está Oculto** para **Sim** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image38.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image38.png)

   _As colunas foram ocultadas porque são usadas por relacionamentos ou serão usadas na configuração de segurança em nível de linha ou lógica de cálculo._

   \*Você usará **SalesOrderNumber** em um cálculo no laboratório **Criar cálculos DAX no Power BI Desktop, Parte 1 .\***

4. Selecione as três colunas a seguir:
   - Produto | Custo padrão
   - Vendas | Custo
   - Vendas | Vendas
5. No painel **Propriedades , dentro da seção Formatação** , defina a propriedade Casas **Decimais como 0** (zero).

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image39.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image39.png)

## **Exercício 3: Revise a Interface do Modelo**

Neste exercício, você alternará para a visualização Relatório e revisará a interface do modelo.

### **Tarefa 1: revise a interface do modelo**

Nesta tarefa, você alternará para a visualização Relatório e revisará a interface do modelo.

1. Mude para a visualização Relatório.
2. No painel **Campos , observe o seguinte:**
   - Colunas, hierarquias e seus níveis são campos, que podem ser usados para configurar visuais de relatório
   - Apenas os campos relevantes para a criação de relatórios são visíveis
   - A tabela **SalespersonRegion** não está visível porque todos os seus campos estão ocultos
   - Os campos espaciais na tabela **Região** e **Revendedor** são adornados com um ícone espacial
   - Os campos adornados com o símbolo sigma (Ʃ) serão resumidos, por padrão
   - Uma dica de ferramenta aparece ao passar o cursor sobre **Vendas |** Campo de **custo**
3. Expanda as **Vendas | OrderDate** e, em seguida, observe que ele revela uma hierarquia de datas.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image40.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image40.png)

   _Os **alvos | O campo TargetMonth** fornece uma hierarquia semelhante. Essas hierarquias não foram criadas por você. Eles foram criados automaticamente. Há um problema, no entanto. O ano financeiro da Adventure Works começa em 1º de julho de cada ano. Mas, nessas hierarquias de datas criadas automaticamente, o ano da hierarquia de datas começa em 1º de janeiro de cada ano._

   _Agora você desativará esse comportamento automático. No laboratório **Criar Cálculos DAX no Power BI Desktop, Parte 1** , você usará o DAX para criar uma tabela de datas e configurá-la para definir o calendário do Adventure Works._

4. Para desativar a hora automática/data, clique na guia da faixa de opções **Arquivo** para abrir a exibição dos bastidores.
5. À esquerda, selecione **Opções e configurações** e, em seguida, selecione **Opções** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image41.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image41.png)

6. Na janela **Opções** , à esquerda, no grupo **Arquivo Atual** , selecione **Carregamento de Dados** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image42.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image42.png)

7. Na seção **Inteligência de tempo** , desmarque **Data/hora automática** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image43.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image43.png)

8. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image44.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image44.png)

9. No painel **Campos** , observe que as hierarquias de datas não estão mais disponíveis.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image45.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image45.png)

## **Exercício 4: Crie Medidas Rápidas**

Neste exercício, você criará duas medidas rápidas.

### **Tarefa 1: crie medidas rápidas**

Nesta tarefa, você criará duas medidas rápidas para calcular o lucro e a margem de lucro.

1. No painel **Campos , clique com o botão direito do mouse na tabela Vendas** e selecione **Nova Medida Rápida** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image46.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image46.png)

2. Na janela **Medidas Rápidas , na lista suspensa Cálculo** , de dentro do grupo **Operações Matemáticas** , selecione **Subtração** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image47.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image47.png)

3. No painel **Campos da janela Medidas Rápidas** , expanda a tabela **Vendas .**
4. Arraste o campo **Vendas para a caixa Valor Base** .
5. Arraste o campo **Custo para a caixa Valor a ser subtraído** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image48.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image48.png)

6. Clique **em OK** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image49.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image49.png)

   \*Uma medida rápida cria a fórmula de cálculo para você. Eles são fáceis e rápidos de criar para cálculos simples e comuns. Você criará medidas sem usar essa ferramenta no laboratório **Criar Cálculos DAX no Power BI Desktop, Parte 1 .\***

7. No painel **Campos , dentro da tabela Vendas** , observe essa nova medida.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image50.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image50.png)

   _As medidas são adornadas com o ícone da calculadora._

8. Para renomear a medida, clique com o botão direito do mouse e selecione **Renomear** .

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image51.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image51.png)

   _Dica: Para renomear um campo, você também pode clicar duas vezes nele ou selecioná-lo e pressionar **F2** ._

9. Renomeie a medida para **Lucro** e pressione **Enter** .
10. Na tabela **Vendas** , adicione uma segunda medida rápida, com base nos seguintes requisitos:

    - Use a operação matemática de **divisão**
    - Defina o **numerador** para as **vendas |** Campo **de lucro**
    - Defina o **denominador** para **vendas |** Campo de **vendas**
    - Renomeie a medida como **Margem de lucro**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image52.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image52.png)

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image53.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image53.png)

11. Certifique-se de que a medida **Margem** de lucro esteja selecionada e, na faixa contextual **Ferramentas de medida** , defina o formato como **Porcentagem** , com duas casas decimais.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image54.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image54.png)

12. Para testar as duas medidas, primeiro selecione o visual da tabela na página do relatório.
13. No painel **Campos , verifique as duas medidas.**

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image55.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image55.png)

14. Clique e arraste a guia direita para ampliar o visual da tabela.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image56.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image56.png)

15. Verifique se as medidas produzem resultados razoáveis que estão formatados corretamente.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image57.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/03-configure-data-model-in-power-bi-desktop_image57.png)

### **Tarefa 2: Crie um relacionamento muitos-para-muitos**

Nesta tarefa, você criará um relacionamento muitos-para-muitos entre a tabela **Vendedor** e a tabela **Vendas** .

1. No Power BI Desktop, na exibição Relatório, no painel **Campos** , verifique os dois campos a seguir para criar um visual de tabela:

   - Vendedor | Vendedor
   - Vendas | Vendas

   _Os laboratórios usam uma notação abreviada para fazer referência a um campo. Ficará assim: **Vendedor | Vendedor** . Neste exemplo, **Vendedor** é o nome da tabela e **Vendedor** é o nome do campo._

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image9.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image9.png)

   _A tabela exibe as vendas realizadas por cada vendedor. No entanto, há outra relação entre vendedores e vendas. Alguns vendedores pertencem a uma, duas ou possivelmente mais regiões de vendas. Além disso, as regiões de vendas podem ter vários vendedores atribuídos a elas._

   _De uma perspectiva de gerenciamento de desempenho, as vendas de um vendedor (com base em seus territórios atribuídos) precisam ser analisadas e comparadas com as metas de vendas. Você criará relacionamentos para apoiar essa análise no próximo exercício._

2. Observe que Michael Blythe vendeu quase US $ 9 milhões.
3. Alterne para a visualização Modelo.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image10.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image10.png)

4. Arraste a tabela **SalespersonRegion** para posicioná-la entre as tabelas **Region** e **Salesperson .**
5. Use a técnica de arrastar e soltar para criar os dois relacionamentos de modelo a seguir:

   - **Vendedor | EmployeeKey** to **SalespersonRegion | EmployeeKey**
   - **Região | SalesTerritoryKey** to **SalespersonRegion | Chave de território de vendas**

   _A tabela **SalespersonRegion** pode ser considerada uma tabela de ponte._

6. Alterne para a exibição Relatório e observe que o visual não foi atualizado — o resultado de vendas de Michael Blythe não foi alterado.
7. Volte para o modo de exibição Modelo e siga as instruções do filtro de relacionamento (ponta de seta) da tabela **Vendedor .**

   _Considere que a tabela **Vendedor** filtra a tabela **Vendas** . Ele também filtra a tabela **SalespersonRegion** , mas não continua propagando filtros para a tabela **Region** (a ponta da seta está apontando na direção errada)._

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image11.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image11.png)

8. Para editar o relacionamento entre as tabelas **Region** e **SalespersonRegion** , clique duas vezes no relacionamento.
9. Na janela **Editar relacionamento , na lista suspensa Direção de filtro cruzado** , selecione **Ambos** .
10. Marque a caixa de seleção **Aplicar filtro de segurança em ambas as direções** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image12.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image12.png)

11. Clique **em OK** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image13.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image13.png)

12. Observe que o relacionamento tem uma ponta de seta dupla.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image14.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image14.png)

13. Alterne para o modo de exibição de relatório e observe que os valores de vendas ainda não foram alterados.

    _O problema agora está relacionado ao fato de que existem dois caminhos de propagação de filtro possíveis entre as tabelas **Vendedor** e **Vendas .** Essa ambiguidade é resolvida internamente, com base em uma avaliação de “menor número de tabelas”. Para ser claro, você não deve projetar modelos com esse tipo de ambiguidade — o problema será abordado em parte posteriormente neste laboratório e pela conclusão do laboratório **Criar cálculos DAX no Power BI Desktop, Parte 1** ._

14. Alterne para a visualização Modelo.
15. Para forçar a propagação do filtro por meio da tabela de ponte, edite (clique duas vezes) o relacionamento entre as tabelas **Vendedor** e **Vendas .**
16. Na janela **Editar relacionamento , desmarque a caixa de seleção Tornar este relacionamento ativo** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image15.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image15.png)

17. Clique **em OK** .

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image16.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image16.png)

    _A propagação do filtro agora seguirá o único caminho ativo._

18. No diagrama, observe que o relacionamento inativo é representado por uma linha tracejada.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image17.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image17.png)

19. Alterne para a visualização Relatório e observe que as vendas de Michael Blythe agora são de quase US$ 22 milhões.

    ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image18.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image18.png)

20. Observe também que as vendas de cada vendedor - se adicionadas - excederiam o total da tabela.

    _É uma observação comum de uma relação muitos-para-muitos devido à contagem dupla, tripla, etc. dos resultados de vendas regionais. Considere Brian Welcker, o segundo vendedor listado. Seu valor de vendas é igual ao valor total de vendas. É o resultado correto simplesmente pelo fato de ele ser o Diretor de Vendas; suas vendas são medidas pelas vendas de todas as regiões._

    _Enquanto o relacionamento muitos-para-muitos está funcionando, agora não é possível analisar as vendas feitas por um vendedor (porque o relacionamento está inativo). Você poderá reativar o relacionamento quando introduzir uma tabela calculada que permitirá analisar as vendas feitas nas regiões de vendas atribuídas ao vendedor (para análise de desempenho) no laboratório **Criar cálculos DAX no Power BI Desktop, Parte 1** ._

21. Alterne para o modo Modelagem e, no diagrama, selecione a tabela **Vendedor .**
22. No painel **Propriedades , na caixa Nome** , substitua o texto por **Vendedor (Desempenho)** .

    _A tabela renomeada agora reflete sua finalidade: é usada para relatar e analisar o desempenho dos vendedores com base nas vendas de suas regiões de vendas atribuídas._

### **Tarefa 3: Relacionar a tabela de Destinos**

Nesta tarefa você criará um relacionamento com a tabela **Destinos**

1. Criar um relacionamento do **Vendedor (Desempenho) |** coluna **EmployeeID e os destinos |** Coluna **CódigoDoFuncionário .**
2. Na visualização Relatório, adicione os **Destinos | Campo de destino** para o visual da tabela.
3. Redimensione o visual da tabela para que todas as colunas fiquem visíveis.

   ![https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image19.png](https://raw.githubusercontent.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/Main/Instructions/Linked_image_Files/04-configure-data-model-in-power-bi-desktop-advanced_image19.png)

   _Agora é possível visualizar vendas e metas, mas tome cuidado por dois motivos. Primeiro, não há filtro em um período de tempo e, portanto, as metas também incluem valores de metas futuras. Em segundo lugar, as metas não são aditivas e, portanto, o total não deve ser exibido. Eles podem ser desabilitados formatando o visual ou removidos usando a lógica de cálculo. Você seguirá a segunda abordagem criando uma medida de destino no laboratório **Criar Cálculos DAX no Power BI Desktop, Parte 2** , que retornará BLANK quando mais de um vendedor for filtrado._

### **Tarefa 4: Concluir**

Nesta tarefa, você concluirá o laboratório.

1. Salve o arquivo do Power BI Desktop.
2. Se solicitado a aplicar consultas, clique em **Aplicar mais tarde** .
3. Se você pretende iniciar o próximo laboratório, deixe o Power BI Desktop aberto.

# **Parabéns!**
