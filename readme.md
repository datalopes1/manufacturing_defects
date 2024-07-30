# Análise Exploratória de Dados - Manufacturing Defects Dataset 

Este dataset contém informações simuladas relacionadas a defeitos de fabricação observados durante os processos de controle de qualidade. Inclui informações como tipo de defeito, data de detecção, localização dentro do produto, nível de gravidade, método de inspeção utilizado e custos de reparo. 

Este conjunto de dados pode ser usado para analisar padrões de defeitos, melhorar os processos de controle de qualidade e avaliar o impacto dos defeitos na qualidade do produto e nos custos de produção. Os dados podem ser encontrados no [Kaggle](https://www.kaggle.com/datasets/fahmidachowdhury/manufacturing-defects) e foram disponibilizados por [Fahmida](https://www.kaggle.com/fahmidachowdhury).

![](https://i.imgur.com/F2h7Tme.jpeg)

## Features
|Coluna|Descrição|
|---|---|
|defect_id|Identificador único do defeito|
|product_id|ID do produto associado com o defeito|
|defect_type|Categória do defeito (cósmetico, funcional ou estrutural)|
|defect_description|Descrição do defeito|
|defect_date|Data de quando o defeito ocorreu|
|defect_location|Local onde o defeito foi encontrado (superficie, componente)|
|severity|Severidade do defeito (pequena, moderada, crítica)|
|inspection_method|Método de inspeção (inspeção visual, teste automatizado)|
|repair_action|Ação tomada para o reparo|
|repair_cost|Custo do reparo|

## Metas e objetivos
A meta deste projeto é através de uma exploração dos dados identificar tendências nos defeitos e outros insights. 

**Uma pequena observação**: Como o conjunto de dados é simulado, irei utilizar como moeda o Real Brasileiro. 

### Resultados
#### Sobre os produtos

- Os Produtos 63, 81, 97, 56,  4, 10, 92,  6, 45, 74 são os que apresentam maior quantidade de defeitos;
- 63 e 81 apresentam valores extremos na frequência de defeitos;
- O Produto 81 além de ser o que mais frequentemente apresenta defeitos, é o que causou mais prejuízos com reparos.

#### Sobre os defeitos

- Defeitos estruturais são os mais frequentes e apresentam tendência de aumento na frequência, equanto os oturos estão em baixa;
- Defeitos de severidade crítica estão com uma tendência de aumento em frequência, o restante apresenta tendência de baixa;
- Existe um ciclo de melhora/piora em relação a frequência de defeitos que deve ser investigado; 
- A superífcie é o local de mais frequente ocorrência de defeitos, com destaque para defeitos estrurais;
- Os defeitos de menor severidade são os mais frequentes.

#### Insights

Vejo a necessidade de realizar um mapeamento do processo de produção e aplicar processos de controle de qualidade como o DMAIC do Six Sigma, para buscar a causa raíz das falhas estrurais na produção dos componentes de Superfície dos produtos. Um caminho apontado pela análise é começar pela investigação do que vem causando os ciclos de aumento e queda do número de defeitos nos Produtos com foco (1) em defeitos de severidade crítica, (2) defeitos do tipo estrurais que estão em tendência de crescimento, antes que os outros aspectos também aumentem a frequência de defeitos, e (3) nos defeitos na superfície dos produtos. 

### Ferramentas utilizadas
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)

### Biblitoecas Python utilziadas
#### Manipulação de dados
- Pandas, NumPy.
#### EDA
- Seaborn, Matplotlib.

# Análise Exploratória de Dados (EDA)
WIP