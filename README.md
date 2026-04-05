# Garimpa.Ai

## Sobre o Projeto

Garampa.Ai é um sistema de consulta de moveis usados com integração da Inteligencia Artificial parta fazer consulta de produtos apartir de Fotos e extrair informações apra ajduar a preificar o produto final restaurado ou resconstruidos.

O sistema foi desenvolvido para marceneiros e restauradores de moveis que precisam ajuda na precificação dos seus serviçoes ou produtos.

Ele utiliza de configurações de consulta do produtos a partir de uma foto, onde ele vai analisar em um banco de lojas virtuais diversar, tentar pegar no maximo 5 referencias de lojas e no minimo 3. Caso não encontre o produto exato ele vai procurar pelo produto mais similiar, respeitando todas as referencias das fotos anexadas para consulta.

### A consulta vai funcionar da seguinte forma

1. *O sistema vai **analisar 3 fotos de ângulos diferentes** do produto em um banco de lojas virtuais usando IA.*
2. *Pegar as Seguintes informações e salvar em variaveis respectivas: **Nome do Produto**; **Link da Vitrine**; **Valor de Venda**.*
3. *Repetir esse processo no minimo 3 e no maximo 5 vezes e armazenar em uma variavel pai com o **Nome da Loja***
4. *Somar todos os valores e dividir pela quantidade de consultas realizadas, o resultado será a média do produto, que vai salvar em uma nova vareavel e apresentra a médio de preço de venda do produto.*

### Possiveis problemas que presicam ser resolvidos

1. Não localizar o produto.
2. Quantidade de Consultas abaixo do minimo.
3. Carregar as imagens do produtocom baixa qualidade.
4. A falta de imagens do produto

Para esses possiveis erros apresentaremos uma mensagem amigavel apr ao usuário:

```txt
Por falta de infomrações, não foi possivel localizar o produto
```
