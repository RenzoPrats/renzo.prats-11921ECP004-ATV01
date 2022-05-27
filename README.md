# Resumo
Para a realização desse projeto foram necessários 4 elementos:

## startup.c
Para construir o startup.c seguimos os seguintes passos :
<ul>
  <li>declaração e inicialização do Stack</li>
  <li>declaração e inicialização da Tabela de Vetores de Interrupção;</li>
  <li>código do Reset handler;</li>
  <li>outros códigos exception handler.</li>
<ul>
  
## main.c
Posteriormente, criamos o main.c que contém a criação de fato do script para piscar o LED, foi realizado os seguintes passos:
<ul>
  <li>Configuração do Reset and Clock Control (RCC)</li>
  <li>Configuração do pino PC13 onde será inserido o LED, é necessário defini-lo como saída push-pull</li>
  <li>Ajustar a utilização do registrador GPIOx_BSRR - GPIO port bit set/reset register que permite alterar o estado do pino de saída de forma atômica</li>
<ul>

## stm32f411-rom.ld (Arquivo linker)
  
Para criação do arquivo linker foi necessário a configuração dos seguintes elementos:
  
<ul>
  <li>ENTRY</li>
  <li>MEMORY</li>
  <li>SECTION</li>
<ul>
    
## Makefile
  
Este arquivo foi criado para automatização do processo de compilação, nele definimos váriaveis e regras de compilação, incluindo a parte de adicionar o linker na compilação.
  
 
