# Usando algoritmo de clustering para analisar padrões de compra

**Considere a seguinte situação:**

Você é analista de dados em uma loja on-line que quer entender os padrões de compra de seus clientes. Essa loja possui dados sobre várias características dos clientes(valor médio gasto, frequência de compra, categorias...), porém nenhum desses dados possuem rótulos que indique quais grupos de clientes existem. 
Nosso objetivo é segmentar os clientes em grupos usando um algoritmo de clustering!

---
Em Python, esse repositório irá gerar um Dataset sintético com o mínimo de 300 registros de clientes, onde irá conter pelo menos 3 features(valor médio gasto, frequência de compra, categorias...) e será feito a normalização desses dados e definiremos k = 4 clusters para implementar o K-Means.

O K-means é um algoritmo simples e eficiente para segmentar clientes em grupos baseados em características numéricas contínuas, como valor gasto, frequência e diversidade de produtos. Ele agrupa os dados em clusters com centróides, facilitando a interpretação dos grupos.

#### Vantagens:
- Fácil de implementar e interpretar.   
- Rápido em datasets com tamanho moderado, como esse com 300 clientes
- Produz clusters esféricos que, neste contexto, ajudam a entender perfis típicos de consumo

#### Limitações:
- É necessário definir previamente o número de clusters. Aqui, escolhemos 4 clusters, mas a escolha pode precisar de análise mais detalhada
- Sensível a outliers, que podem distorcer a posição dos centróides.
- Assume que clusters são convexos e aproximadamente do mesmo tamanho.

## Output previsto:

![clusters](https://github.com/user-attachments/assets/e68bf00b-9073-46ef-b91e-03be6cc6e2cd)

Cada cluster representa um grupo de clientes com comportamento de compra similar, por exemplo:
- Clientes que gastam pouco, compram pouco e em poucas categorias.
- Clientes que gastam muito, compram frequentemente e em várias categorias.
- Clientes intermediários, etc.

Com essa segmentação, a loja pode criar estratégias personalizadas, como promoções direcionadas, campanhas específicas para cada perfil, ou até melhorar o sortimento de produtos para grupos mais diversificados.

