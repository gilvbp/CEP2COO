# Transformar CEP em latitude e longitude

A fun��o `cep2coo()` transforma o  CEP em dados de latitude e longitude. A fun��o usa recursos do Python para consultar a API dos Correios e R para consultar as coordenadas no [Open Street Map](https://www.openstreetmap.org) (OSM).

A consulta � API dos correios � feita pela fun��o da biblioteca [pycep-correios](https://pypi.org/project/pycep-correios/) escrita em python.

Ap�s obter informa��es de endere�o e cidade � feita uma consulta da latitude e longitude no OSM com a fun��o `geocode` do pacote [photon](https://github.com/rCarto/photon) escrito para o R.


## Exemplo

`cep2coo("20090003") # -22.90369 -43.1782`

O resultado da latitude e longitude apresentar� *missing value* se o CEP for inv�lido.


