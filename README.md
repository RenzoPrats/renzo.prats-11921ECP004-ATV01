# Resumo
Para a realização desse projeto foram necessários 4 elementos:

## startup.c
Para construir o startup.c seguimos os seguintes passos :
* declaração e inicialização do Stack
* declaração e inicialização da Tabela de Vetores de Interrupção;
* código do Reset handler;
* outros códigos exception handler.

  
## main.c
Posteriormente, criamos o main.c que contém a criação de fato do script para piscar o LED, foi realizado os seguintes passos:
* Configuração do Reset and Clock Control (RCC)
* Configuração do pino PC13 onde será inserido o LED, é necessário defini-lo como saída push-pull
* Ajustar a utilização do registrador GPIOx_BSRR - GPIO port bit set/reset register que permite alterar o estado do pino de saída de forma atômica

## stm32f411-rom.ld (Arquivo linker)
  
Para criação do arquivo linker foi necessário a configuração dos seguintes elementos:
  
* ENTRY
* MEMORY
* SECTION
    
## Makefile
  
Este arquivo foi criado para automatização do processo de compilação, nele definimos variáveis e regras de compilação, incluindo a parte de adicionar o linker na compilação.
  
 
