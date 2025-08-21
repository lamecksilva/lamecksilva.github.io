# Computer Systems: A Programmer's Perspective

**21/08/2025**

Um sistema de computador consiste de hardware e software de sistemas que rodam juntos para rodar aplicações.  
Aplicações específicas dos sistemas mudam com o tempo, mas os conceitos internos não.

---

## Informação é Bits + Contexto

Um programa de hello world ganha vida como código fonte quando o programador o cria com um editor e salva em um arquivo de texto chamado hello.c.

```c
# include <stdio.h>

int main() {
  printf("hello, world\n");
  return 0;
}
```

Arquivos de texto são sequências de bits, cada um com valor 0 ou 1, agrupados em grupos de 8-bit chamados bytes. Cada byte representa algum caractere do texto no programa.

O programa hello.c é guardado em um arquivo como uma sequência de bytes. Cada byte tem um valor inteiro que corresponde a algum caractere.

Arquivos de texto são os que consistem exclusivamente de ASCII caracteres. Todos outros arquivos são incluídos como arquivos binários.

Toda informação em um sistema, incluindo arquivos em disco, programas armazenados na memória, dados de usuários guardados na memória, dados transmitidos na rede, são representados como uma sequência de bits.

A única coisa que diferencia diferentes bytes de dados é o contexto que usamos eles. Em diferentes contextos, a mesma sequência de bytes pode representar um inteiro, string, número de ponto flutuante ou instruções de máquina.

---

Como programadores precisamos entender como as máquinas representam números, porque eles não são o mesmo que inteiros e números reais.  
Eles são pontos aproximados que podem se comportar de maneiras inesperadas.
