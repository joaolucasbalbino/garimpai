# GarimpAi

## Sobre o Projeto

GarampAi é um sistema de consulta de moveis usados com integração da Inteligencia Artificial parta fazer consulta de produtos apartir de Fotos e extrair informações apra ajduar a preificar o produto final restaurado ou resconstruidos.

O sistema foi desenvolvido para marceneiros e restauradores de moveis que precisam ajuda na precificação dos seus serviçoes ou produtos.

Ele utiliza de configurações de consulta do produtos a partir de uma foto, onde ele vai analisar em um banco de lojas virtuais diversar, tentar pegar no maximo 5 referencias de lojas e no minimo 3. Caso não encontre o produto exato ele vai procurar pelo produto mais similiar, respeitando todas as referencias das fotos anexadas para consulta.

A consulta vai funcionar da seguinte forma:

1. *O sistema vai analisar 3 fotos de ângulos diferentes do produto em um banco de lojas virtuais usando IA.*
2. *Pegar as Seguintes informações e salvar em variaveis respectivas: Nome do Produto; Link da Vitrine; Valor de Venda.*
3. *Repetir esse processo no minimo 3 vezes e no maximo 5 e armazenar em uma variavel pai com o Nome da Loja*
4. *Somer todos os valores e dividir pela quantidade de consultas, o resultado será a média do produto*
