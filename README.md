# Garimpa.Ai

## Sobre o Projeto

Garampa.Ai é um sistema de consulta de moveis usados com integração da Inteligencia Artificial parta fazer consulta de produtos apartir de Fotos e extrair informações apra ajduar a preificar o produto final restaurado ou resconstruidos.

O sistema foi desenvolvido para marceneiros e restauradores de moveis que precisam ajuda na precificação dos seus serviçoes ou produtos.

Ele utiliza de configurações de consulta do produtos a partir de uma foto, onde ele vai analisar em um banco de lojas virtuais diversar, tentar pegar no maximo 5 referencias de lojas e no minimo 3. Caso não encontre o produto exato ele vai procurar pelo produto mais similiar, respeitando todas as referencias das fotos anexadas para consulta.

## Funcionalidades do Sistema

### 1. Analise de Imagens com IA

O usuário vai carregar um conjunto de fotos para serem analisadas com Inteligencia Artificial. A quantidade minima de fotos que devem ser carregadas é de 3 fotos, se possivel de angulos diferentes. Não tem um valor maximo, quanto mais fotos melhor o refinamento da consulta.

As imagens precisam estar com uma qualidade minima para o sistema fazer a consulta, caso a imagem esteja muito a baixo, o sistema vai apresentar uma mensagem de erro:

```text
As imagens carregadas estão com  baixa resolução, isso pode comprometer na consulta do produto!
```

### 2. Variaveis de Consulta

Durante o processo de analise das fotos, o sistema deve encontrar as seguintes informações no banco de lojas virtuais:

1. *Imagen do Produto*;
2. *Nome do Produto*;
3. *Link da Vitrine*;
4. *Valor de Venda*.

Essas informmações vão ficar salvas em variaveis de igual nome para serem apresentadas em uma lista de comparação após a consulta.

### 3. Looping de consultas

O Sistema vai fazer esse processo no minimo 3 e no maximo 5 vezes, e sempre que ele fizer este processo ele vai salvar em uma variavel pai com o nome da Loja. Assim todas as consultas ficam listadas de forma separada para fazer a comparação dos valores em diferentes lojas.

### 4. Média de Preço Sugerido

Após realizar as consultas e salvar nas devidas variaveis, o sistema vai fazer uma soma de todos os valores e depois dividir pela quantidade de consultas, o resultado será o o valore de venda sugerido ao usuário.

## Possiveis problemas

+ **Não localizar o produto.**
  + **Como Resolver:** Encontrar o produto mais similar possivel, sempre respeitando, as caracteristas do produto.

+ **Quantidade de Consultas abaixo do minimo.**
  + **Como Resolver:** Apresentar a seguinte pensagem *"Por falta de informações, não foi possivel localizar o produto"*

+ **A falta de imagens do produto.**
  + **Como Resolver:** Tentar consultar com a quantidade fornecida, porém, avisar o usuário final que isso pode comprometer na consulta do Produto.

+ **As fotos serem diferentes.**
  + **Como Resolver:** Não realizar a consulta por divergencia do produto.
