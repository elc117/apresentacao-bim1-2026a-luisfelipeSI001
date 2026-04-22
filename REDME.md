# Apresentação Luis Felipe – Prolog (Listas e Logic Puzzles)

## 1 - Parte Teórica -

1. ### Estrutura de listas (cabeça e cauda)
   
Listas em Prolog seguem o formato `[Cabeça | Cauda]`, onde a cabeça é o primeiro elemento e a cauda é o restante da lista.

2. ### Listas homogêneas e heterogêneas

Listas em Prolog não precisam ter todos os elementos do mesmo tipo.

✔️ Exemplo de lista homogênea:

[1,2,3,4]

Exemplo de lista heterogênea:

[1, teste, X, movie(1, parasite, 2019)]

3. ### Predicados com listas 

O uso de predicados como `member`, `length` e `list_to_set`, que facilitam trabalhar com listas.

---

### member/2
Verifica se um elemento pertence a uma lista.

Formato: member(Elemento, Lista).
Exemplo:
member(3, [1,2,3,4]).

Resultado:
true.

Também pode gerar valores:
member(X, [a,b,c]).

Resultado:

X = a

X = b

X = c


## length/2
Retorna o tamanho de uma lista.

Formato:
length(Lista, Tamanho).
Exemplo:
length([1,2,3,4], N).

Resultado:

N = 4.

## list_to_set/2

Remove elementos repetidos de uma lista.

Formato:
list_to_set(Lista, ListaSemRepeticao).
Exemplo:
 
list_to_set([a,a,b,c,c], R).

Resultado:

R = [a,b,c].

---

##  Parte Prática

###  Exploração do arquivo `movies.pl`

O programa contém informações sobre:
- Filmes (`movie/3`)
- Atores (`actor/2`)
- Atrizes (`actress/2`)
- Gêneros (`genre/2`)
- Curtidas (`likes/2`)

---

##  Exercícios

### 1. O filme schindlers_list é uma comédia?

```prolog
genre(9, comedy).

!(assets/prolog1.gif)
