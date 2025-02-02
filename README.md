<h1 align="center">
    <img alt="Banner" title="#Banner" style="object-fit: cover; height:250px;" src=".github/banner.png" />
</h1>

# ✨ Tarefa04-Interrupcoes

<p align="center"> Repositório dedicado a Tarefa 04 do processo de capacitação do EmbarcaTech que envolve interrupções na placa Raspberry Pi Pico W por meio da Placa BitDogLab.</p>

## 📌 Índice
<p align="center">    
  <a href="#apresentacao-da-tarefa"> Apresentacao da tarefa </a> &nbsp; &nbsp; &nbsp; | &nbsp; &nbsp; &nbsp;        
  <a href="#objetivos"> Objetivos </a> &nbsp; &nbsp; &nbsp; | &nbsp; &nbsp; &nbsp;          
  <a href="#descricao-do-projeto"> Descricao do Projeto </a> &nbsp; &nbsp; &nbsp; | &nbsp; &nbsp; &nbsp;  
  <a href="#integrantes-do-projeto"> Integrantes do Projeto </a> &nbsp; &nbsp; &nbsp; | &nbsp; &nbsp; &nbsp;  
  <a href="#funcionamento-do-projeto"> Funcionamento do Projeto </a> &nbsp; &nbsp; &nbsp; | &nbsp; &nbsp; &nbsp;         
  <a href="#gif-mostrando-o-funcionamento-do-programa-na-placa-bitdoglab"> GIF mostrando o funcionamento do programa na placa BitDogLab </a> &nbsp; &nbsp; &nbsp; | &nbsp; &nbsp; &nbsp;        
  <a href="#video-no-youtube-mostrando-o-funcionamento-do-programa-na-placa-bitdoglab"> Video no youtube mostrando o funcionamento do programa na placa BitDogLab </a>
</p>

## :clipboard: Apresentacao da tarefa

Para consolidar a compreensão dos conceitos relacionados ao uso de interrupções no microcontrolador RP2040 e explorar as funcionalidades da placa de desenvolvimento BitDogLab, esta atividade propõe a implementação de um projeto prático envolvendo controle de LEDs e tratamento de eventos com botões.

## :dart: Objetivos

- Compreender o funcionamento e a aplicação de interrupções em microcontroladores;

- Implementar a técnica de debouncing via software para eliminar o efeito de bouncing em botões;

- Manipular e controlar LEDs comuns e LEDs endereçáveis WS2812;

- LED RGB deve piscar 5 vezes por segundo.

## :books: Descricao do Projeto

Utiizou-se a placa BitDogLab (que possui o microcontrolador RP2040) para o controle de LEDs endereçáveis WS2812 por meio de interrupções, esses por sua vez são acionados por meio de botões (Botão A no GPIO 05 e Botão B no GPIO 06).
O funcionamento da interrupção ocorre por meio da API de Hardware *gpio_set_irq_enabled* que opera de forma externa ao processamento central, não afetando o funcionamento do LED RGB, que deve piscar 5 vezes por segundo.

## :walking: Integrantes do Projeto

- Matheus Pereira Alves

## :bookmark_tabs: Funcionamento do Projeto

- O LED RGB (como é utilizado o GPIO 13, será o vermelho) irá piscar 5 vezes por segundo;
- A Matriz de LEDs 5x5 iniciará com o valor 0 printado;
- O Botão A incrementa o valor mostrado na matriz de 0 a 9;
- O Botão B decrementa o valor mostrado na matriz de 9 a 0.

## :camera: GIF mostrando o funcionamento do programa na placa BitDogLab
<p align="center">
  <img src=".github/GIFdemo.gif" alt="GIF" width="345px" />
</p>

## :arrow_forward: Video no youtube mostrando o funcionamento do programa na placa BitDogLab

<p align="center">
    <a href="https://www.youtube.com/watch?v=iAumEOQ9L48">Clique aqui para acessar o site</a>
</p>



