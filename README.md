# Análise do clima de Nova Iguaçu


[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)


# Tabela de conteúdos
- [Introdução](#introdução)
- [Como usar](#como-usar)
- [Configurações recomendadas](#configurações-recomendadas)
- [Relatório no Power BI](#relatório-no-power-bi)

# Introdução
[Voltar ao topo](#tabela-de-conteúdos)

Um código feito para analisar a temperatura máxima e mínima durante a semana em Nova Iguaçu, RJ.

O código foi feito utilizando o Google Collab, e nele será possível calcular a mínima/máxima temperatura e a média das temperaturas. O site utilizado para a raspagem dos dados do dia e da temperatura foi o [tempo.com](https://www.tempo.com/nova-iguacu.htm).

# Como usar
[Voltar ao topo](#tabela-de-conteúdos)

Para fazer a raspagem de outro local, basta procurar a localidade que esta procurando no [tempo.com](https://www.tempo.com/nova-iguacu.htm) e mudar o link do requests:
````
r = requests.get('novoLink')
````

# Configurações recomendadas
[Voltar ao topo](#tabela-de-conteúdos)

Para que o programa funcione é necessário fazer o download e a importação das seguintes bibliotecas:
- requests (Para conseguir pegar a URL)
- bs4 (Para a utilização do BeautifulSoup)
- pandas (Para a transformação dos dados em DataFrame)
- google.colab (Para baixar o arquivo csv)

Para a importação é necessário utilizar o código abaixo:
````
import requests
import re
import pandas as pd
from bs4 import BeautifulSoup
from google.colab import files
````


# Relatório no Power Bi
[Voltar ao topo](#tabela-de-conteúdos)

Para uma melhor visualização dos dados eu transformei o DataFrame em um arquivo csv e fiz um relátorio no Power BI:

![Relatorio](https://github.com/TinyHero13/climaNovaIguacu/blob/main/assets/relatorio.png)
