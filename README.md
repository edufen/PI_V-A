# PI_V-A
Projeto Integrador V-A [PUC-GO]

# Análise de Dados sobre Queimadas no Brasil

## INTRODUÇÃO

As queimadas no Brasil representam um desafio significativo para a conservação ambiental, a biodiversidade e a gestão sustentável de recursos naturais. Com uma vasta extensão de florestas e ecossistemas únicos, o país enfrenta a crescente ameaça dos incêndios florestais, que não apenas devastam áreas verdes, mas também afetam diretamente a qualidade do ar, a saúde pública e o clima global.

Nos últimos anos, o aumento das queimadas, muitas vezes associado a práticas agrícolas e à exploração desenfreada dos recursos naturais, levantou preocupações em nível nacional e internacional sobre a sustentabilidade e a preservação dos nossos biomas.

Este trabalho tem como objetivo analisar dados sobre queimadas, utilizando técnicas avançadas de visualização de dados em ferramentas de Business Intelligence e Data Science. Através da análise dos dados disponíveis no Banco de Dados de Queimadas (BDQueimadas) do Instituto Nacional de Pesquisas Espaciais (INPE), busca-se não apenas quantificar a incidência de incêndios, mas também investigar a complexa relação entre variáveis climáticas como, precipitação, dias sem chuva e FRP.

Ao oferecer insights detalhados sobre esses fatores, pretende-se contribuir para uma compreensão mais profunda e abrangente do fenômeno das queimadas no Brasil. Através dessa análise, espera-se fornecer subsídios para a formulação de políticas públicas mais eficazes e estratégias de manejo sustentável, visando a mitigação dos impactos ambientais e a promoção de práticas que respeitem a integridade dos ecossistemas.

Este estudo, portanto, não apenas se propõe a mapear e entender o comportamento das queimadas, mas também a gerar reflexões sobre a importância da conscientização e da ação coletiva para a preservação do nosso patrimônio natural.

---

## DESENVOLVIMENTO

Os dados utilizados neste estudo foram coletados a partir do Banco de Dados de Queimadas (BDQueimadas), uma aplicação WebGIS mantida pelo Instituto Nacional de Pesquisas Espaciais (INPE). Para garantir a integridade e a relevância dos dados analisados, utilizou-se a linguagem de programação Python, que oferece uma série de bibliotecas poderosas para o tratamento e a limpeza de dados.

### Limpeza dos Dados

A etapa de limpeza dos dados envolveu vários passos fundamentais, incluindo a padronização das siglas dos estados, a conversão das horas para o formato `datetime` e a remoção de outliers e dados irrelevantes. Esses passos foram essenciais para assegurar a consistência e a usabilidade das informações. As colunas selecionadas para o dashboard incluíram:

- **Data e Hora**: Horário de referência da passagem do satélite.
- **Cidade, Estado, País e Município**: Informações geográficas que ajudam a contextualizar as queimadas.
- **Bioma**: Identificação do bioma afetado, crucial para entender os impactos ecológicos.
- **Dias Sem Chuva e Precipitação**: Indicadores climáticos que podem influenciar a ocorrência de incêndios.
- **Risco de Fogo**: Classificação do risco de incêndio.
- **Latitude e Longitude**: Coordenadas geográficas das ocorrências, permitindo o mapeamento preciso.
- **FRP (Fire Radiative Power)**: Mede a energia radiante liberada por unidade de tempo, refletindo a intensidade do fogo.

### Análise dos Dados

A análise permitiu identificar a relação entre variáveis climáticas e a ocorrência de queimadas. Esta relação foi evidenciada nas diferentes páginas do dashboard, que abordaram temas como a quantidade de queimadas por bioma e a relação entre precipitação e risco de fogo. Essas análises fornecem insights valiosos para compreender os fatores que contribuem para a incidência de incêndios florestais.

---

## Visualização no Power BI

O dashboard no Power BI foi dividido em quatro páginas, cada uma focando em aspectos distintos das queimadas:

1. **Queimadas no Brasil**: Uma visão geral das ocorrências de queimadas em diferentes regiões.
   
   _Imagem: Gráfico de barras mostrando a quantidade de queimadas por estado._
   
2. **Relação Climática e Risco de Incêndio**: Análise que correlaciona as variáveis climáticas com os níveis de risco de incêndio.
   
   _Imagem: Gráfico de dispersão entre precipitação e risco de incêndio._
   
3. **Intensidade dos Incêndios**: Avaliação da intensidade das queimadas, utilizando dados de FRP.
   
   _Imagem: Mapa do Brasil com as intensidades de FRP por região._
   
4. **Dias Sem Chuvas**: Uma análise da influência da precipitação na ocorrência de incêndios.
   
   _Imagem: Gráfico de linha mostrando a relação entre dias sem chuvas e focos de queimadas._

Cada página do dashboard permite filtragens por mês, estado e bioma, proporcionando uma análise detalhada e interativa que pode ser utilizada para apoiar a tomada de decisões em políticas de gestão ambiental.

---

## CONCLUSÃO

A análise dos dados de queimadas no Brasil em 2024 evidencia a eficácia das técnicas de visualização na compreensão de fenômenos complexos. Este estudo não apenas mapeia as queimadas, mas também estabelece uma base sólida para futuras investigações e políticas de conservação.

Os biomas mais afetados foram:

- **Amazônia**: Registrando um total alarmante de 87.054 focos de incêndio.
- **Cerrado**: Com 56.107 focos.
- **Mata Atlântica**: 14.385 focos.
  
As regiões Norte, Centro-Oeste e Nordeste foram as mais impactadas, com **Mato Grosso** liderando em número total de queimadas (22,52%), seguido por **Pará** (17,07%) e **Amazonas**.

A média de risco de incêndios variou conforme a precipitação, destacando áreas mais vulneráveis, e os dados indicam tendências significativas que merecem atenção em futuras análises.

A **Potência Radiativa do Fogo (FRP)** revelou que o Pantanal teve os maiores índices de intensidade de incêndios, indicando incêndios de longa duração, seguido por Cerrado e Amazônia.

A correlação entre o número de dias sem chuva e as queimadas reforça a importância da precipitação na mitigação do risco de incêndios, com áreas mais secas apresentando maior vulnerabilidade.

---

## INSIGHTS

### Total de Queimadas por Bioma

- **Amazônia**: 87.054 focos (maior devastação).
- **Cerrado**: 56.107 focos (predisposição às queimadas devido ao clima).
- **Mata Atlântica**: 14.385 focos.
- **Pantanal**: 10.377 focos (preocupante, dada sua menor extensão territorial).

_Imagem: Gráfico de barras comparando as queimadas por bioma._

### Total de Queimadas por Região

- A região Norte apresentou a maior proporção de queimadas, destacando uma severa crise climática.
- O Centro-Oeste também enfrentou uma crise crescente, exacerbada por correntes de vento que transportam fumaça, piorando a qualidade do ar e impulsionando mais queimadas.
  
_Imagem: Mapa de calor destacando as queimadas por região._

### Focos de Incêndio por Estado

- **Mato Grosso** lidera em porcentagem de focos de incêndio (22,52%).
- **Pará** segue com 17,07%.
- **Amazonas** vem em terceiro com 10,95%.

_Imagem: Mapa do Brasil com a quantidade de focos por estado._

### Intensidade dos Incêndios

O **Pantanal** lidera em Potência Radiativa do Fogo (FRP), indicando incêndios de grande intensidade e duração.

_Imagem: Gráfico de barras mostrando a intensidade dos incêndios por bioma._

### Dias Sem Chuvas

A relação é clara: mais dias sem chuvas aumentam o risco de incêndios e a intensidade (alta FRP), mostrando que a vegetação seca é um combustível para as chamas.

_Imagem: Gráfico de linha entre dias sem chuvas e focos de incêndio._
