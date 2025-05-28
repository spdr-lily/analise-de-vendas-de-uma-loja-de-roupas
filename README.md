## **Projeto de Análise de Dados de Vendas de Loja de Roupas**

#### **1\. Introdução**

Este projeto visa realizar uma análise de dados de vendas de uma loja de roupas. O objetivo é analisar os dados de vendas para gerar informações relevantes sobre a quantidade vendida, o valor total arrecadado e o preço médio dos produtos vendidos.

#### **2\. Metodologia**

O projeto foi desenvolvido utilizando a Python e as bibliotecas Pandas, NumPy e Matplotlib. As etapas incluem:

1. **Importação das Bibliotecas:** As bibliotecas Pandas, NumPy e Matplotlib foram importadas para manipulação e análise dos dados, além da criação de visualizações gráficas.  
2. **Criação do DataFrame:** Um DataFrame foi gerado com 1000 linhas, contendo informações sobre o ID do produto, nome do produto, quantidade vendida, preço unitário e data da venda. Os nomes dos produtos foram definidos em uma lista e selecionados aleatoriamente para preencher a coluna `Nome Produto`.  
3. **Salvamento e Carregamento do Arquivo CSV:** O DataFrame foi salvo em um arquivo CSV (`vendas.csv`) e, em seguida, carregado novamente para garantir a persistência dos dados e a capacidade de trabalhar com eles.  
4. **Análise Descritiva:** A função `describe()` foi utilizada para obter estatísticas descritivas do conjunto de dados, como média, desvio padrão, mínimo, máximo e quartis das colunas numéricas.  
5. **Acesso e Manipulação de Colunas:**  
   * Acesso a colunas foi realizado utilizando `.loc` para selecionar a coluna `ID Produto`.  
   * A função `map` foi aplicada para transformar os nomes dos produtos para letras maiúsculas.  
   * A ordenação do DataFrame foi feita pela coluna `Preço Unitario` em ordem decrescente.  
6. **Agrupamento e Cálculo de Média:** Os dados foram agrupados pela coluna `Nome Produto` e a média das colunas numéricas foi calculada para cada produto, fornecendo insights sobre a média de vendas e preços por produto.  
7. **Seleção e Remoção de Dados:**  
   * A seleção de linhas foi realizada para filtrar o DataFrame onde `ID Produto` é igual a 2\.  
   * Duplicatas foram removidas do DataFrame para garantir a integridade dos dados.  
8. **Acesso com `iloc`:** Acesso a colunas foi feito utilizando `iloc` para selecionar a segunda coluna (`Nome Produto`).  
9. **Cálculo da Média de Vendas por Produto:** A média de vendas para cada produto foi calculada agrupando os dados por `Nome Produto` e calculando a média da `Quantidade Vendida`.  
10. **Acesso a Célula Específica:** O valor de uma célula específica (segunda linha e quarta coluna) foi acessado para demonstrar a manipulação de dados em nível de célula.  
11. **Salvamento do DataFrame Modificado:** O DataFrame modificado foi salvo em um novo arquivo CSV (`vendas_modificado.csv`).  
12. **Visualização dos Dados:**  
    * Gráficos de barras foram gerados para visualizar a quantidade média vendida e o preço médio por produto.

#### **3\. Resultados**

Os principais resultados do projeto incluem:

* **Média de Vendas por Produto:** A média de vendas foi calculada para cada produto, permitindo identificar os produtos mais vendidos.  
* **Preço Médio por Produto:** O preço médio de cada produto foi determinado, auxiliando na análise de precificação.

#### **4\. Conclusão**

Este projeto forneceu uma análise detalhada dos dados de vendas da loja de roupas, abordando a quantidade vendida e o preço médio dos produtos. Os resultados obtidos podem ser utilizados para tomada de decisões estratégicas, como gestão de estoque e precificação.
