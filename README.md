# Desafio 1 — Sistema de Votação

**O que o programa faz:**
Simula uma votação entre Ana, Bruno e Carlos. O usuário digita os votos um por um, e no final o programa mostra quantos votos cada um recebeu e quem ganhou.

**Estruturas utilizadas:**

| Estrutura | Como foi usada |
|---|---|
| **Lista** | Armazena todos os votos digitados. Ex: `['Ana', 'Bruno', 'Ana']` |
| **if/else** | Verifica se o voto digitado é válido antes de registrar |
| **.count()** | Conta quantas vezes um candidato aparece na lista de votos |

**Métodos utilizados:**

| Método | Sintaxe | O que faz |
|---|---|---|
| **.append()** | `lista.append(item)` | Adiciona um item no final da lista |
| **.count()** | `lista.count(item)` | Retorna quantas vezes o item aparece na lista |
| **.capitalize()** | `texto.capitalize()` | Deixa a primeira letra maiúscula e o resto minúsculo |
| **max()** | `max(valores)` | Retorna o maior valor de um conjunto de valores |

**Como rodar:**
```
python desafio_01_votacao.py
```

**Exemplo:**
```
Entrada:  Ana, Bruno, Ana, Fim
Saída:    Ana: 2 votos | Bruno: 1 voto | Carlos: 0 votos
          Vencedor: Ana
```

---

# Desafio 2 — Editor de Texto com Desfazer

**O que o programa faz:**
Funciona como um bloco de notas simples. O usuário digita palavras e pode apagar a última caso cometa um erro — igual ao `Ctrl+Z` de um editor de texto.

**Estruturas utilizadas:**

| Estrutura | Como foi usada |
|---|---|
| **Lista (Pilha)** | Guarda as palavras digitadas em ordem. Ex: `['casa', 'azul', 'bonita']` |
| **LIFO** | O último item adicionado é o primeiro a ser removido — igual a uma pilha de pratos |
| **.append()** | Adiciona a nova palavra no **final** da lista |
| **.pop()** | Remove e retorna o **último** item da lista, simulando o desfazer |

**Métodos utilizados:**

| Método | Sintaxe | O que faz |
|---|---|---|
| **.append()** | `lista.append(item)` | Adiciona um item no final da lista |
| **.pop()** | `lista.pop()` | Remove e retorna o **último** item da lista |
| **.join()** | `' '.join(lista)` | Une todos os itens da lista em uma única string separada por espaço |
| **enumerate()** | `enumerate(lista, 1)` | Percorre a lista retornando o índice e o valor de cada item |

**Como rodar:**
```
python desafio_02_editor_pilha.py
```

**Exemplo:**
```
Entrada:  1→"casa", 1→"azul", 2 (desfaz), 3 (mostrar)
Saída:    Texto atual: casa
```

---

# Desafio 3 — Fila de Atendimento

**O que o programa faz:**
Simula uma fila de atendimento, como em um banco ou hospital. Quem chega primeiro é atendido primeiro.

**Estruturas utilizadas:**

| Estrutura | Como foi usada |
|---|---|
| **Lista (Fila)** | Guarda os nomes das pessoas na ordem em que chegaram. Ex: `['João', 'Maria', 'Pedro']` |
| **FIFO** | O primeiro item adicionado é o primeiro a ser removido — igual a uma fila de pessoas |
| **.append()** | Adiciona a nova pessoa no **final** da fila |
| **.pop(0)** | Remove e retorna o **primeiro** item da lista, chamando quem chegou primeiro |

**Métodos utilizados:**

| Método | Sintaxe | O que faz |
|---|---|---|
| **.append()** | `lista.append(item)` | Adiciona um item no **final** da fila |
| **.pop(0)** | `lista.pop(0)` | Remove e retorna o **primeiro** item da lista |
| **.join()** | `' '.join(lista)` | Une todos os itens da lista em uma única string separada por espaço |
| **len()** | `len(lista)` | Retorna a quantidade de itens dentro da lista |

**Como rodar:**
```
python desafio_03_fila_atendimento.py
```

**Exemplo:**
```
Entrada:  1→"João", 1→"Maria", 2 (chamar), 3 (ver fila)
Saída:    Chamando: João
          Fila atual: Maria
```

---

> 💡 **Diferença entre Pilha e Fila:**
> - **Pilha (LIFO)** — como uma pilha de pratos: você sempre pega o de **cima** (último que entrou)
> - **Fila (FIFO)** — como uma fila de banco: você sempre atende o da **frente** (primeiro que entrou)

> 📌 **Diferença entre .pop() e .pop(0):**
> - **.pop()** — remove o **último** item (usado na pilha)
> - **.pop(0)** — remove o **primeiro** item (usado na fila)
