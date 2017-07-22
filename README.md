# Ajuda o busão

A idéia desse projeto é indicar a melhor rota considerando :
* uma distância máxima à ser percorrida
* uma lista de pontos intermediários que pode ser atendidas ou não
* um número máximo de pontos

## Exemplo de situação

* Um ônibus quer sair do ponto A até o ponto B
* Existem pessoas nos pontos intermediários C, D e E
* O ônibus pode percorrer no máximo uma distância K
* Uma solução para esse problema é uma rota que saí de A até B, passando por pontos (X, Y, Z) de modo que as distâcias C-X, D-Y e E-Z sejam iguais (com um erro e). Essa rota deve ter uma distância K
* Outra solução é que a rota escolhida atenda o maior número de pontos possível

## Abordagens possíveis

* Criar um ponto médio de pontos que estejam próximos à menos de uma distância (k)
  * Utilizar algoritmo de clustering k-means?
  * Nessa solução o número de grupos pode ser o número máximo de pontos de parada
