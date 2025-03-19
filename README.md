# Projeto de um processador RISC-V multiciclo

Nesse projeto, os alunos desenvolverão um processador RISC-V simples multiciclo. A intenção principal é dominar questões básicas do desenvolvimento de hardware, como a definição de um conjunto de instruções, a implementação da máquina de estados de um processador multiciclo e a verificação do funcionamento do processador.

## Objetivos

1. Implementar um processador RISC-V simples multiciclo em Verilog sintetizável. 
2. Implementar um conjunto de testes para verificar o funcionamento do processador.
3. Executar programas implementados em C no processador.

## Especificação

Seu processador deve implementar as instruções RV32I, que é o conjunto mais simples de instruções RISC-V. A implementação deve ser multiciclo, ou seja, cada instrução pode levar um número diferente de ciclos de clock para ser executada. Você pode se inspirar na implementação multiciclo do livro "Computer Organization and Design" de David Patterson e John Hennessy.

Você pode utilizar um toolchain pronto ou montar o seu próprio toolchain ([dica de geração](https://github.com/riscv-collab/riscv-gnu-toolchain)). Alternativamente, para esse primeiro trabalho, você pode utilizar um montador [online](https://riscvasm.lucasteske.dev) (existem outros, fique à vontade para utilizar o que achar mais conveniente).

Como método de encerramento do programa, você pode utilizar a instrução *ebreak*, que encerra o simulador.

Seu código deve ser sintetizávelvel, isso significa que deve ser possível gerar um circuito lógico a partir do seu código. A verificação será feita através do iverilog.

