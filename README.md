# Atividade-em-C

Comandos De Entrada 

1) Qual a biblioteca e necessário com diretiva  # indude para ultilizar as funções de entrada padrão da linguagem C?

Para utilizar as funções de entrada e saída padrão na linguagem C, você deve incluir a biblioteca `<stdio.h>`. O diretiva `#include <stdio.h>` fornece as declarações necessárias para funções como `printf`, `scanf`, `fgets`, e `fprintf`, entre outras.
Aqui está um exemplo básico:
```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

2)O trecho de código Realiza a leitura de um número InteIRO Entretanto, ele contém dols ERROS. CORRIJa-os e Justi fique sua Resposta int n, sconf ("%f", n);
O trecho de código que você forneceu contém erros. Vamos corrigi-los e explicar as correções:

### Código Original com Erros
```c
int n, sconf ("%f", n);
```

### Problemas Identificados
1. **Uso incorreto de `scanf`**: A função `scanf` está escrita de forma incorreta e usa o especificador de formato errado para ler um número inteiro.
2. **Falta de ponto e vírgula no final da linha**: A linha está faltando o ponto e vírgula (`;`), que é necessário para terminar a instrução.
3. **Especificador de formato incorreto**: Para ler um número inteiro, você deve usar `%d` em vez de `%f`.

### Código Corrigido
```c
#include <stdio.h>

int main() {
    int n; // Declaração da variável para armazenar o número inteiro
    printf("Digite um número inteiro: ");
    scanf("%d", &n); // Correção: uso do especificador de formato %d e do operador & para ler o valor
    printf("Você digitou: %d\n", n); // Exemplo de como você pode usar a variável lida
    return 0;
}
```

### Explicação das Correções
1. **Incluir a biblioteca `<stdio.h>`**: Para usar `printf` e `scanf`, você deve incluir a biblioteca padrão de entrada e saída com `#include <stdio.h>`.
2. **Correção do `scanf`**: O especificador de formato para ler um número inteiro é `%d`, e você deve passar o endereço da variável (`&n`) para `scanf` para que ela possa armazenar o valor lido na variável `n`.
3. **Adição do ponto e vírgula**: Cada instrução em C deve terminar com um ponto e vírgula.

Assim, o código corrigido lê um número inteiro da entrada padrão e o exibe.

3)Exdique o trecho de código abaixo (linha 2)
Char C sconf("%c", &Cl, While (getchar() != "I'm'),
Char C sconf("%c", &Cl, While (getchar() != "I'm'),
#include <stdio.h>

int main() {
    char c; // Declara uma variável do tipo char
    printf("Digite um caractere: ");
    scanf("%c", &c); // Lê um caractere da entrada padrão e armazena em 'c'

    // Leitura e descarte de caracteres adicionais até encontrar uma nova linha
    while (getchar() != '\n'); 

    // Exibe o caractere lido
    printf("Você digitou: %c\n", c);
    return 0;
}

4)Explique o trecho de códigu abaixo float largura, comprimento, scamf ("%f %f, delargura, & comprimental]
float largura, comprimento, scamf ("%f %f, delargura, & comprimental
#include <stdio.h>

int main() {
    float largura, comprimento; // Declaração das variáveis para armazenar os valores de ponto flutuante

    // Solicita ao usuário que insira dois valores
    printf("Digite a largura e o comprimento: ");
    
    // Lê dois valores de ponto flutuante da entrada padrão
    scanf("%f %f", &largura, &comprimento);

    // Exibe os valores lidos
    printf("Largura: %.2f\n", largura);
    printf("Comprimento: %.2f\n", comprimento);

    return 0;
}

5)Explique o trecho de codigy abaixo Char, nome [80],

scanf("%s", nome),

1. **`char nome[80];`**
   - Esta linha declara um array de caracteres chamado `nome` com capacidade para armazenar até 80 caracteres. Em C, um `char` é um tipo de dado usado para armazenar um único caractere, e um array de `char` é frequentemente usado para armazenar strings (sequências de caracteres).

2. **`scanf("%s", nome);`**
   - `scanf` é uma função usada para ler entrada do usuário. O formato `"%s"` indica que estamos esperando ler uma string (sequência de caracteres). 
   - `nome` é o endereço do array onde a string lida será armazenada. A função `scanf` lerá caracteres até encontrar um espaço em branco, uma quebra de linha ou o final do input, e armazenará esses caracteres no array `nome`.

Então, o código está configurado para ler uma string de até 79 caracteres (o 80º caractere é reservado para o caractere nulo `'\0'` que marca o fim da string) e armazená-la no array `nome`. Se a string inserida pelo usuário for maior que 79 caracteres, `scanf` pode causar um estouro de buffer, o que pode levar a comportamentos indesejados ou vulnerabilidades de segurança.

6)Explique o trecho de código abaixo pantf ("Ola, mundo"),
Parece que há um pequeno erro de digitação no trecho de código fornecido. A função correta que você deve estar tentando usar é `printf`, não `pantf`. 

Aqui está a explicação corrigida para `printf`:

**`printf("Olá, mundo");`**

- **`printf`** é uma função em C usada para imprimir dados na tela. 
- **`"Olá, mundo"`** é uma string literal que será exibida na tela. 

Quando o código `printf("Olá, mundo");` é executado, ele simplesmente exibe a mensagem "Olá, mundo" no console. 

Se você quiser um exemplo de código completo que usa essa função, ele se pareceria com isto:

```c
#include <stdio.h>

int main() {
    printf("Olá, mundo");
    return 0;
}
```

Neste exemplo, a função `printf` é chamada dentro da função `main`, que é o ponto de entrada de um programa em C. Quando o programa é executado,ele

7)abaixo (linha 2)

Char C sconf("%c", &Cl, While (getchar() != "I'm'),

Explique o trecho de códigu abaixo float largura, comprimento, scamf ("%f %f, delargura, & comprimental]

5) Explique o trecho de codigy abaixo Char, nome [80],

scanf("%s", nome),

Explique o trecho de código abaixo pantf ("Ola, mundo"),

Explique o trecho de código abouro Dica Ja Resposta nás é a mesma da questão anterior.

printf("Oda, mundo! In"),
Char C sconf("%c", &Cl, While (getchar() != "I'm'),
char c;
scanf("%c", &c);
while (getchar() != '\n');
float largura, comprimento;
scanf("%f %f", &largura, &comprimento);
char nome[80];
scanf("%s", nome);
pantf ("Ola, mundo"),
printf("Olá, mundo");
printf("Oda, mundo! In"),
printf("Olá, mundo");
printf("Oda, mundo! In"),
printf("Olá, mundo!\n");
printf("Olá, mundo!\n");

8)Explique o trecho de código abaixo

Printf("1+1m)
Printf("1+1m)
printf("1+1\n");
O trecho de código fornecido está incorreto, mas parece que você está tentando usar a função `printf` para imprimir uma expressão ou uma string. Vou corrigir e explicar o que o código deveria ser:

**Código fornecido:**

```c
Printf("1+1m)
```

**Correção:**

```c
printf("1+1\n");
```

**Explicação:**

- **`printf`**: Função em C usada para imprimir texto no console. O nome da função é `printf`, não `Printf` (o `p` deve ser minúsculo).
- **`"1+1\n"`**: String literal que será exibida na tela. 

  - **`"1+1"`**: A string contém os caracteres `1`, `+`, e `1`, exatamente como são escritos.
  - **`\n`**: Caractere de nova linha que move o cursor para a linha seguinte após imprimir a string. Isso é opcional e só é necessário se você quiser que o cursor vá para a próxima linha.

Quando você executa o código corrigido:

```c
printf("1+1\n");
```

Ele imprimirá:

```
1+1
```
