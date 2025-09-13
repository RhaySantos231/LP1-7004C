# LP1-7003C
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
---

## 📂 Lista de Atividades
- [Lista 1 – Variáveis, Operadores Matemáticos e if/else](https://docs.google.com/document/d/1pfy5TH6OVX3XXufT9q3VN0aSqXCmTJGxGbD22tK6Ixw/edit?usp=sharing)
