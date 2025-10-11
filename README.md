# LP1-7004C
# Principais Comandos Git

| Comando | Descrição |
|---------|-----------|
| `git init` | Inicializa um novo repositório Git na pasta atual |
| `git clone <url>` | Clona um repositório remoto para a máquina local |
| `git status` | Mostra o estado atual dos arquivos (modificados, não rastreados etc.) |
| `git add <arquivo>` | Adiciona um arquivo específico para a área de staging |
| `git add .` | Adiciona **todos os arquivos modificados** para a área de staging |
| `git commit -m "mensagem"` | Registra as mudanças adicionadas com uma mensagem |
| `git log` | Mostra o histórico de commits |
| `git branch` | Lista todas as branches (ramificações) |
| `git branch <nome>` | Cria uma nova branch |
| `git checkout <nome>` | Troca para a branch especificada |
| `git merge <nome>` | Mescla a branch especificada com a branch atual |
| `git remote -v` | Mostra os repositórios remotos configurados |
| `git push origin <branch>` | Envia os commits locais para o repositório remoto |
| `git pull origin <branch>` | Atualiza a branch local com alterações do remoto |
| `git fetch` | Busca atualizações do repositório remoto **sem mesclar** |
| `git reset --hard <hash>` | Reseta o repositório para um commit específico (perigoso, pois apaga alterações locais) |

---

📌 **Dica para alunos iniciantes**:  
A sequência mais comum é:  
```bash
git add .
git commit -m "Mensagem explicativa"
```


# Introdução a Linguagem de Programação Kotlin

## Vantagens:
- Criado pela JetBrains em 2011.

- Oficialmente suportado pelo Google para Android desde 2017.

- Estaticamente tipada (tipos definidos em tempo de compilação).

- Pode ser usada em Android, backend, desktop e web.

- Interoperável com Java (funciona junto no mesmo projeto).

- Sintaxe simples e enxuta, com menos código repetitivo.

- Suporta POO e programação funcional.


# Tipos de Variáveis em Kotlin

| Tipo       | Descrição | Exemplo |
|------------|-----------|---------|
| `Int`      | Números inteiros (32 bits) | `val idade: Int = 20` |
| `Long`     | Números inteiros longos (64 bits) | `val populacao: Long = 7500000000` |
| `Short`    | Números inteiros curtos (16 bits) | `val numero: Short = 30000` |
| `Byte`     | Números inteiros pequenos (8 bits) | `val b: Byte = 120` |
| `Double`   | Números decimais (64 bits, maior precisão) | `val peso: Double = 70.5` |
| `Float`    | Números decimais (32 bits, menor precisão) | `val altura: Float = 1.75f` |
| `Char`     | Um único caractere | `val letra: Char = 'A'` |
| `String`   | Texto (sequência de caracteres) | `val nome: String = "Maria"` |
| `Boolean`  | Valores lógicos (true / false) | `val ativo: Boolean = true` |

---

📌 **Dica:**  
- Use `val` para variáveis **imutáveis** (constantes).  
- Use `var` para variáveis **mutáveis** (que podem mudar de valor).  

# Operadores Matemáticos em Programação

## Principais Operadores

1. **`+` (Adição)** → Soma valores.  
   Exemplo: `5 + 3 = 8`

2. **`-` (Subtração)** → Subtrai valores.  
   Exemplo: `10 - 4 = 6`

3. **`*` (Multiplicação)** → Multiplica valores.  
   Exemplo: `6 * 2 = 12`

4. **`/` (Divisão)** → Divide valores.  
   Exemplo: `15 / 3 = 5`

5. **`%` (Módulo ou Resto da Divisão)** → Retorna o resto de uma divisão.  
   Exemplo: `10 % 3 = 1`


# Estruturas Condicionais (if / else)

O `if` e o `else` são usados para tomar decisões no programa.  
Eles verificam uma condição (verdadeira ou falsa) e executam o bloco correspondente.

## Exemplos

1. **If/else simples**  
```kotlin
val idade = 18

if (idade >= 18) {
    println("Você é maior de idade")
}else{
    println("Você é menor de idade")
}
```
## ✅ If/Else Composto (`else if`)

Use quando você precisa **avaliar várias condições diferentes**, e não apenas duas opções.

### Exemplo em Kotlin:
```kotlin
val nota = 75

if (nota >= 90) {
    println("Excelente!")
} else if (nota >= 70) {
    println("Bom desempenho")
} else if (nota >= 50) {
    println("Precisa melhorar")
} else {
    println("Reprovado")
}
```
# Estruturas de Repetição em Kotlin

As estruturas de repetição permitem executar um bloco de código várias vezes, enquanto uma condição for verdadeira. Em Kotlin, as principais estruturas são `while` e `do/while`.

---

## Estrutura `while`

O `while` executa o bloco de código **enquanto a condição for verdadeira**.  
A condição é verificada **antes** de cada execução.

### Sintaxe básica
```kotlin
while (condicao) {
    // código a ser repetido
}
```
## 2. Estrutura `do/while`

O `do/while` executa o bloco **pelo menos uma vez**, e só depois verifica a condição.  
Isso garante que o bloco seja executado mesmo que a condição seja falsa no início.

### Sintaxe
```kotlin
do {
    // código a ser repetido
} while (condicao)
```
# Estrutura `when`

O `when` é uma estrutura de controle de fluxo em Kotlin, semelhante ao `switch` de outras linguagens, mas mais poderosa. Ele permite executar diferentes blocos de código dependendo do valor de uma expressão.

---

## Sintaxe básica

```kotlin
when (expressao) {
    valor1 -> {
        // código a ser executado se expressao == valor1
    }
    valor2 -> {
        // código a ser executado se expressao == valor2
    }
    else -> {
        // código a ser executado se nenhum valor corresponder
    }
}
```
---
# Operadores de Comparação em Kotlin

| Operador | Significado             | Exemplo em Kotlin   | Resultado |
|----------|-------------------------|---------------------|-----------|
| >        | Maior que               | `5 > 3`             | `true`    |
| <        | Menor que               | `2 < 7`             | `true`    |
| >=       | Maior ou igual          | `5 >= 5`            | `true`    |
| <=       | Menor ou igual          | `4 <= 6`            | `true`    |
| ==       | Igualdade entre valores | `10 == 10`          | `true`    |
| !=       | Diferente de            | `8 != 3`            | `true`    |

---
# 📘 Introdução — Arrays e Listas em Kotlin

## 🔹 O que é um Array?

Um **Array** é uma estrutura que armazena **vários valores do mesmo tipo** em uma única variável.  
Cada elemento possui um **índice**, começando em **0**.

### Exemplo:
```kotlin
val numeros = arrayOf(10, 20, 30, 40)
println(numeros[0]) // Exibe 10
```
> ⚠️ **Importante:** O tamanho de um `array` é **fixo** — depois de criado, **não pode ser alterado**.

---

## 🔹 O que é uma List?

Uma **List** é parecida com um `Array`, mas **mais flexível**.  
Existem dois tipos principais:

- `listOf()` → **imutável** (não pode adicionar ou remover itens)  
- `mutableListOf()` → **mutável** (permite adicionar, remover, modificar)

---

### Exemplo:

```kotlin
val frutas = mutableListOf("Maçã", "Banana", "Laranja")
frutas.add("Melancia")       // Adiciona
frutas.remove("Banana")      // Remove
println(frutas[0])           // Exibe "Maçã"
```
# 🧩 Comandos de Manipulação de List em Kotlin

| 💻 Comando / Método | 📝 Descrição | 🧠 Exemplo em Kotlin |
|----------------------|--------------|-----------------------|
| `listOf()` | Cria uma **lista imutável** (não pode ser modificada) | `val frutas = listOf("Maçã", "Banana")` |
| `mutableListOf()` | Cria uma **lista mutável** (permite alterações) | `val frutas = mutableListOf("Maçã", "Banana")` |
| `add(item)` | Adiciona um novo item à lista | `frutas.add("Laranja")` |
| `add(index, item)` | Adiciona um item em uma posição específica | `frutas.add(1, "Uva")` |
| `remove(item)` | Remove o item especificado | `frutas.remove("Banana")` |
| `removeAt(index)` | Remove o item na posição informada | `frutas.removeAt(0)` |
| `clear()` | Remove **todos** os itens da lista | `frutas.clear()` |
| `size` | Retorna o **tamanho da lista** | `println(frutas.size)` |
| `isEmpty()` | Verifica se a lista está vazia (retorna `true` ou `false`) | `frutas.isEmpty()` |
| `contains(item)` | Verifica se um item está presente na lista | `frutas.contains("Maçã")` |
| `get(index)` | Retorna o item de um índice específico | `println(frutas.get(0))` |
| `[index]` | Acessa o item diretamente pelo índice | `println(frutas[1])` |
| `indexOf(item)` | Retorna o índice da primeira ocorrência do item | `println(frutas.indexOf("Laranja"))` |
| `sort()` | Ordena a lista em ordem crescente (alfabética ou numérica) | `frutas.sort()` |
| `reverse()` | Inverte a ordem dos elementos da lista | `frutas.reverse()` |
| `for (item in lista)` | Percorre todos os elementos da lista | `for (f in frutas) println(f)` |
| `joinToString()` | Converte a lista em uma única string formatada | `println(frutas.joinToString(", "))` |

---
## 📂 Lista de Atividades
- [Lista 1 – Variáveis, Operadores Matemáticos e if/else](https://docs.google.com/document/d/1pfy5TH6OVX3XXufT9q3VN0aSqXCmTJGxGbD22tK6Ixw/edit?usp=sharing) (inicio 20/09| fim: 20/09) 
- [Lista 2 – When, while e do while](https://docs.google.com/document/d/1X7piSX--u729lxASkoCxMtXNbnMEUwBYLeS39EWXcGU/edit?tab=t.0#heading=h.bmwx0c14zlpb) (inicio: 27/09 | fim: 04/10)
