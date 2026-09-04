# una-gqs-listaSeis-java

# Algoritmo de Ordenação: Bubble Sort

Este projeto contém uma implementação simples e didática do algoritmo **Bubble Sort** (Ordenação por Bolha) utilizando a linguagem Python.

## O que é o Bubble Sort?
O Bubble Sort é um algoritmo de ordenação básico que percorre a lista repetidamente, comparando elementos adjacentes e trocando-os de lugar caso estejam na ordem errada. Esse processo é repetido até que a lista esteja completamente ordenada.

## Como utilizar

O código recebe uma lista de números desordenados e retorna a mesma lista organizada em ordem crescente.

### Exemplo de código:

```python
def bubble_sort(lista):
    n = len(lista)
    for i in range(n):
        for j in range(0, n - i - 1):
            if lista[j] &gt; lista[j + 1]:
                lista[j], lista[j + 1] = lista[j + 1], lista[j]
    return lista

# Exemplo de uso:
numeros = [64, 34, 25, 12, 22, 11, 90]
ordenados = bubble_sort(numeros)
print(f"Lista ordenada: {ordenados}")
