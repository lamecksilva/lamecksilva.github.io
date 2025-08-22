# CS:APP - GCC

## Programas são traduzidos por outros programas em diferentes formas

Nosso programa _hello.c_ começa em alto nível (porque pode ser lido e
entendido por humanos nessa forma), e para ser executado, as declarações
em C precisam ser traduzidas por outros programas em uma sequência de
instruções de máquina em baixo nível.\
Essas instruções são compactadas em um objeto executável e armazenadas
no disco como um arquivo binário.

```bash
$ gcc -o hello hello.c
```

---

## Fases do sistema de compilação

1. **Pré-processamento**: O pré-processador modifica o arquivo
   original, incluindo os códigos das bibliotecas inseridas, e cria um
   novo arquivo de programa em C.

2. **Compilação**: O compilador traduz o arquivo resultante da fase
   anterior e o traduz para assembly.

3. **Fase de montagem (Assembly phase)**: O assembler (montador) traduz
   o resultado da fase anterior em linguagem de máquina.

4. **Fase de ligação (Linking phase)**: O linker organiza os novos
   códigos em outros módulos (como principais que estão em outros
   binários/arquivos de linguagem de máquina) e faz a união (merge)
   deles, resultando em um arquivo executável que está pronto para ser
   carregado na memória e executado pelo sistema.
