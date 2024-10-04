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

![Screenshot](https://cdn.discordapp.com/attachments/1254451336682930226/1291790983654150144/image.png?ex=6701619a&is=6700101a&hm=cf4456d8ca64bb35c4194aea4e2df8ff6e8624c6860931615fdb1a455296036c&)


- **Amazônia**: 87.054 focos (maior devastação).
- **Cerrado**: 56.107 focos (predisposição às queimadas devido ao clima).
- **Mata Atlântica**: 14.385 focos.
- **Pantanal**: 10.377 focos (preocupante, dada sua menor extensão territorial).

### Total de Queimadas por Região

![Screenshot](https://cdn.discordapp.com/attachments/1254451336682930226/1291791662938329118/image.png?ex=6701623c&is=670010bc&hm=49ec0370e591651cbc9df075fbc99398ff0f884fab1500254480ee9a0d5b6851&)


- A região Norte apresentou a maior proporção de queimadas, destacando uma severa crise climática.
- O Centro-Oeste também enfrentou uma crise crescente, exacerbada por correntes de vento que transportam fumaça, piorando a qualidade do ar e impulsionando mais queimadas.

### Focos de Incêndio por Estado

![Screenshot](https://cdn.discordapp.com/attachments/1254451336682930226/1291791846359695380/image.png?ex=67016268&is=670010e8&hm=72e6cdcd109e4620fba452033e2728c06d232090db00c85745373e7bc6283ec1&)


- **Mato Grosso** lidera em porcentagem de focos de incêndio (22,52%).
- **Pará** segue com 17,07%.
- **Amazonas** vem em terceiro com 10,95%.

### Intensidade dos Incêndios

![Screenshot](https://cdn.discordapp.com/attachments/1254451336682930226/1291792155123126355/image.png?ex=670162b2&is=67001132&hm=60d1ea3b18db827b99c1b957492ffb1ceef852134a7ab281184cb96697763dc8&)

O **Pantanal** lidera em Potência Radiativa do Fogo (FRP), indicando incêndios de grande intensidade e duração.

### Dias Sem Chuvas

![Screenshot](https://cdn.discordapp.com/attachments/1254451336682930226/1291792312350801920/image.png?ex=670162d7&is=67001157&hm=d67b333b6999c326c30e5a8061e3c8a4ecebb532ffbee549c3aa72476a706ba3&)

A relação é clara: mais dias sem chuvas aumentam o risco de incêndios e a intensidade (alta FRP), mostrando que a vegetação seca é um combustível para as chamas.

Página 1
![Screenshot](https://cdn.discordapp.com/attachments/1254451336682930226/1291792918079864904/image.png?ex=67016368&is=670011e8&hm=9dc5e825d93855a75a919454812cdcea61afa20a52d0baf760816003ce35e37c&)

Página 2
![Screenshot](https://cdn.discordapp.com/attachments/1254451336682930226/1291793153833046016/image.png?ex=670163a0&is=67001220&hm=1321ac7ecb93c34d68eb2ebe880ba07610747720432cecaf10333eb84a91c6f6&)

Página 3
![Screenshot](https://cdn.discordapp.com/attachments/1254451336682930226/1291793292039553086/image.png?ex=670163c1&is=67001241&hm=e3f173e4c04d22b2dd136248b2cff1a56f388d4e491da2843ad8e872e8bb1b46&)

Página 4
![Screenshot](https://cdn.discordapp.com/attachments/1254451336682930226/1291793414077153300/image.png?ex=670163de&is=6700125e&hm=8ed0bc2969d56dbed22dc67b2e0c035e5b0b75f27d6f4171d7419835f9c9aff5&)


Dashboards feitos por Jorge Freitas e Julia Aguiar.
