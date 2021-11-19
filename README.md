# MO433
Aprendizado não-supervisionado

## Trabalho 01
### Regras de associação

- Dataset em http://fimi.ua.ac.be/data/retail.dat que é um dataset real de compras no varejo em uma loja na Belgica.
- Regras de associação que tenham suporte mínimo de 0.005 e confiança minima de 0.9.
- [Biblioteca python apyori](https://pypi.org/project/apyori/)

## Trabalho 02
### O objetivo desta tarefa é usar algoritmos e métricas de clusterização da familia de k-means.

1. k-means
    - Rode o kmeans com k de 2 a 15.
    - use silhueta e pelo menos alguma outra medida interna de qualidade
    - moste os graficos dessas medidas versus o k-
2. Escolha um k
    - Discuta usando essas medidas qual é o k que voce escolheria - em princípio nao há uma “resposta certa” para essa questão. Mas alguns K são mais razoáveis que os outros.
3. GMM
    - Usando o k escolhido no item anterior, rode o GMM
    - com gaussianas esféricas (matrizes de covariancia sao a matriz identidade vezes uma constante)
    - com gaussianas diagonais (matrizes de covariancia sao matrizes diagonais)
    - com gaussianas sem restrição (as matrizes de covariancia são livres)
4. Medidas externas para comparar duas clusterizações

    - GMM nao produz uma clustrerização tradicional onde cada dado é associado a UM cluster. Para dado, GMM associa um probabilidade do dado pertencer a cada um dos clusters. Para usar as medidas de concordancia entre clusterizações, as clusterizações precisam.
    - use pelo menos 2 medidas externas para comparar a solução do GMM sem restrição (full) com as outras 2 (esférica e diagonal).
    - reporte os resultados