# Big O Notation

Material utilizado para estudar Big O Notation.
Esse material tem parte do conteúdo em inglês e parte em português.

---

## Definições:

- Complexidade de tempo:
  - É o tanto de tempo utilizado para que um algoritmo seja executado.

- Complexidade de espaço:
  - É o tanto de espaço em memória que será necessária para executar o algoritmo.

- O Big O Notation é uma forma algébrica de verificar o tempo de execução de um determinado código.

---

##  Order of Growth                

Pode ser definida a eficiência de execução dos algoritmos através da order of growth.

|  Order of Growth | Notation    | Definição   |
|------------------|----------   |------------ |
| MELHOR           |             |             |
|                  | O(1)        |Constante    |
|                  | O(log n)    |Logarítmico  |
|                  | O(n)        |Linear       |
|                  | O(n log n)  |Linearitmico |
|                  | O(n²)       |Quadratico   |
|                  | O(n³)       |Cubico       |
|                  | O(2^n)      |Exponencial  |
|                  | O(n!)       |Fatorial     |
| PIOR             |             |             |

---

## Notações

### O(1)

Esse tipo de resultado ocorre quando o tempo de execução é constante, independente do volume de dados de entrada (em uma função por exemplo). 

```py

def mostrar_gato():
  print("🐱")

```

## O(n)

Nesse tipo a execução terá um tempo linear baseado nos dados de entrada. Sendo o melhor tempo quando receber um parâmetro, e o pior quando receber infinitos.

```py

paisagens = ["🌌", "🌇", "🌆"]

def mostrar_paisagem(paisagens: list):
  for paisagem in paisagens:
    print(paisagem)

```

## O(n²)

Tempo que costuma ocorrer em algoritmos que possuem dois loops aninhados onde é necessário acessar todos os elementos dos loops.

```py

paisagens = ["🌌", "🌇", "🌆"]
itens_mar = ["🌊", "⚓", "⛵"]

def combinar_listas(listas: list):
  for paisagem in paisagens:
    for item_mar in itens_mar:
      print(f"# {paisagem} #{item_mar}")
```

## O(2^n)

Caso que ocorre em alguns tipos de algoritmos recursivos e que pode gerar dados que são incrementados até que a condição definida seja atingida.

O exemplo clássico é uma função para montar uma sequência de Fibonacci

```py

def fibonacci(numero: int):
  if(numero <= 1) return numero
  return fibonacci(numero - 2) + fibonacci(numero - 1)
```

## O(log n)

Ocorre quando é necessário iteraração até que uma determinada condição seja atingida, sendo que pode ocorrer antes de iterar em todos objetos da lista

```py

def encontrar_numero_sorte():

numero = 20

while(numero != 100):
  numero = numero * 2
  print(numero)


```

## O(n log n)

Algoritmos que para n elementos executam procedimentos do tipo dividir para conquistar até que a condição seja atingida.

## O(n!)

Esses algorítmos geraram valores exponenciais até que a condição seja atingida. Geralmente possuem recursão em suas estruturas.

## Referências utilizadas:

- Big O Notation - Full Course - FreeCodeCamp - https://www.youtube.com/watch?v=Mo4vesaut8g



