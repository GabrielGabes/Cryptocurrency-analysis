# Projeto Análise de Criptomoedas

Este projeto é uma ampla exploração do mercado de criptomoedas, focada na análise de tendências de crescimento e na correlação com outros mercados. Utilizamos principalmente dados do Yahoo Finance, juntamente com as bibliotecas Seaborn e Pandas, para criar gráficos e tabelas que facilitam a interpretação do mercado de criptomoedas. Estas visualizações e análises nos permitem testar hipóteses e identificar correlações entre valores e eventos distintos.

Este projeto visa obter e analisar dados de criptomoedas utilizando o pacote `yfinance`. As análises incluem cálculos de lucro/perda, mudanças percentuais e visualizações de dados através de histogramas.

## Descrição do Projeto

O projeto é composto por funções que facilitam o download dos dados históricos de criptomoedas e a realização de diversas análises financeiras. Abaixo, estão descritas as principais funcionalidades do projeto:

### Função `crypto_df_download`

Esta função permite o download dos dados históricos de uma criptomoeda específica a partir de um ano inicial definido.

```python
def crypto_df_download(moeda, ano_inicio):
    df = yf.download(moeda, start=str(ano_inicio)+"-01-01", end="2024-06-16")
    cryptos.append(df)
    return df

ano = '2015'

# Defi Famosas
BTC = crypto_df_download("BTC-USD", ano) # 'Bitcoin')
BNB = crypto_df_download("BNB-USD", ano) # 'Binance Coin'
```
