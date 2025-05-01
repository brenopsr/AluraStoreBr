# Alura Store

## Descrição do Projeto  
O projeto **Alura Store** faz parte de um desafio de análise de dados do programa Oracle Next Education. Nele, consolidamos dados de vendas de quatro lojas virtuais (Loja 1 a Loja 4), incluindo informações de produtos, categorias, avaliações de clientes, valores de frete e localização dos pedidos. O objetivo é explorar esses dados de maneira interativa em um *notebook* (Jupyter ou Google Colab) e gerar insights visuais que ajudem na tomada de decisão estratégica para o negócio.

## Objetivo da Análise  
O principal objetivo é identificar padrões e desempenhos entre as lojas para responder à pergunta estratégica: **“Qual loja devemos vender?”**. Analisamos indicadores financeiros (faturamento), perfil de produtos vendidos (categorias e itens mais lucrativos), satisfação dos clientes (avaliações), custos logísticos (frete) e distribuição geográfica das vendas. A ideia é embasar a decisão com dados concretos, destacando pontos fortes e fracos de cada unidade.

## Análise de Dados e Principais Insights

### Faturamento Total por Loja  
 ![image](https://github.com/user-attachments/assets/3e2484da-4b26-4cb8-9d11-2cbb860df2d6)
 A análise revelou que a **Loja 1** obteve o maior faturamento total (aproximadamente R\$ 1,53 milhão), seguida de perto pelas Lojas 2 e 3. A **Loja 4** apresentou o menor faturamento (cerca de R\$ 1,38 milhão). Esse gráfico de barras deixa claro que, apesar das quatro lojas terem escalas de receita semelhantes, a Loja 1 lidera ligeiramente, enquanto a Loja 4 fica atrás das demais. Esses valores sugerem que a Loja 4 pode estar com desempenho financeiro inferior comparado às outras.  

### Vendas por Categoria (Loja 1)  
 ![image](https://github.com/user-attachments/assets/54d041a4-8061-45e1-bbf0-07f634c55ec7)
 A distribuição de vendas da **Loja 1** por categoria mostra que *eletrônicos* correspondem a cerca de **40%** do faturamento, sendo o segmento mais forte. Em seguida vêm *alimentos* (33%) e *roupas* (27%). Esse equilíbrio indica que a Loja 1 tem um portfólio diversificado, mas puxa receita principalmente de eletrônicos. Em análises semelhantes para as outras lojas, pode-se verificar se essa predominância se repete ou se outras categorias ganham relevância em cada local.

### Avaliações vs. Faturamento  
 ![image](https://github.com/user-attachments/assets/fda820d2-8677-4ba9-a389-069601cccf1f)
 Esse gráfico de dispersão relaciona a avaliação média dos clientes e o faturamento por loja. Observa-se que a **Loja 1**, mesmo tendo o maior faturamento, possui a menor avaliação média (em torno de 3,98 estrelas). Por outro lado, a **Loja 3** apresenta a maior avaliação (cerca de 4,05) mas um faturamento ligeiramente menor. Não há uma correlação clara: lojas com avaliações mais altas não necessariamente faturam mais. Isso sugere que fatores além da satisfação imediata do cliente (talvez histórico de produtos ou investimento em marketing) influenciam as vendas. Vale investigar por que a Loja 1 lidera em vendas mesmo com avaliação inferior.

### Produtos Vendidos  
Analisamos também os **produtos mais vendidos** e que mais impactam o faturamento. Descobrimos que itens eletrônicos de alto valor — como televisores e notebooks — foram responsáveis por grande parte da receita nas lojas que mais faturam. Em especial, televisores de alta definição aparecem como *produtos de maior retorno*. Esse insight indica oportunidades: reforçar o estoque desses produtos em lojas com demanda forte e explorar cross-selling (vender produtos relacionados) para maximizar receita. Lojas com menor faturamento podem adotar estratégias semelhantes ou reavaliar o mix de produtos oferecidos.

### Frete e Custos Logísticos  
Outra etapa foi avaliar o **custo médio de frete** para cada loja. Observou-se que a **Loja 1** tem o frete mais caro em média (cerca de R\$ 34,70), enquanto as **Lojas 3 e 4** registram os fretes mais baratos (aproximadamente R\$ 31,30). Custos de frete mais altos podem reduzir a competitividade; portanto, as Lojas 3 e 4 são mais eficientes logisticamente nesse quesito. Para a Loja 1, convém revisar contratos logísticos ou oferecer promoções de frete para não afugentar clientes, especialmente sendo a loja líder em vendas — fretes elevados podem ameaçar esse posto. O frete impacta diretamente o preço final ao cliente e, possivelmente, a satisfação em compras futuras.

### Localização Geográfica das Vendas  
 ![image](https://github.com/user-attachments/assets/57d7a3af-692d-47db-addd-f02e3708ba41)
 Utilizando coordenadas geográficas dos pedidos, construímos um mapa de calor no Brasil. Destacam-se grandes aglomerados ao redor de São Paulo (Sudeste) e na região de Fortaleza (Nordeste). Isso indica que a maior parte das vendas concentra-se nessas regiões, refletindo talvez maior base de clientes ou estratégias locais mais eficazes. Outras capitais brasileiras aparecem com pontos de calor moderado (ex.: Brasília, Rio, BH). Esses padrões geográficos sugerem focar campanhas de marketing e logística no Sudeste e Nordeste, onde a demanda é maior. Em contrapartida, reforçar presença em áreas com baixo calor (Centro-Oeste, Norte) pode ser um plano de expansão ou ajuste de estoques.

## Tecnologias e Bibliotecas Utilizadas  
- **Linguagem:** Python 3.x  
- **Ambiente:** Jupyter Notebook (executado localmente ou no Google Colab)  
- **Bibliotecas:** Pandas (manipulação de dados), Matplotlib/Seaborn (visualizações estáticas), Folium (mapas interativos), NumPy (cálculos numéricos), Geopandas (opcional para mapas)  
- **Outras Ferramentas:** Git para versionamento, Jupyter/Colab para execução, ambiente virtual ou `requirements.txt` para dependências  

## Instruções de Execução  
1. Clone este repositório e acesse a pasta do projeto no terminal.  
2. Abra o notebook `Alura_Store.ipynb` no **Jupyter Notebook** ou faça upload para o **Google Colab**.  
3. Instale as dependências necessárias (por exemplo, `pip install pandas matplotlib folium seaborn` ou use o arquivo `requirements.txt`).  
4. Execute as células sequencialmente. O notebook contém comentários explicativos e visualizações para cada etapa da análise.  
5. Os gráficos serão gerados inline, e o mapa de calor aparecerá interativo (no Colab, pode exigir habilitar a visualização do Folium).

## Conclusão e Recomendações  
Com base nos dados analisados, a **Loja 4** apresenta os indicadores mais fracos: menor faturamento total e custos logísticos relativamente altos, sem destaque em nenhuma categoria de produtos. Por esses motivos, **recomenda-se vender a Loja 4**, pois ela traz o pior desempenho geral para o grupo. As outras lojas (especialmente a Loja 1) têm faturamento maior e poderiam manter a operação de forma mais lucrativa. Ressalta-se, porém, que a Loja 1 apresenta pontos de atenção (frete elevado e avaliação de clientes menor), e pode demandar ações de melhoria. 

Em resumo, a análise suporta a decisão de alienar a Loja 4. Para as demais, sugere-se aproveitar os insights obtidos (como foco em eletrônicos de alta demanda e estratégias nas regiões de maior concentração) para aumentar vendas e satisfação. A decisão final, porém, fica amparada por dados concretos destacados neste relatório.

 ![image](https://github.com/user-attachments/assets/60274469-3136-4fbb-bb9b-43e958e27190)
