---
layout: post-page
title: Navegação com Algortmo Dijkstra
subtitle: ' "Navegar é preciso" '
cover-img: /assets/img/2021-12-20-turtlebot-dijkstra/cover12.jpg
thumbnail-img: /assets/img/2021-12-20-turtlebot-dijkstra/turtlebotPi.jpg
share-img: /assets/img/rosa-logo-redondo.png
author: Matheus Anselmo
tags: [blog]
comments: true
---
## Navegação com Utilizando o Algortmo

### Sobre navegação autônoma

A navegação é uma funcionalidade importante para a robótica móvel. Esta funcionalidade, como o próprio nome já sugere, permite aos robôs móveis a capacidade de se deslocar em ambientes, externos e/ou internos. A navegação comunalmente pode ser realizada por teleoperação ou de forma autônoma. Na teleoperação, há necessidade de um humano realizar o controle de movimento dos robôs móveis, em outras palavras, por meio de um joystick ou um instrumento de comunicação, um operador  guia o robô. Na navegação autônoma, não há presença humana  no deslocamento do robô.
 
A navegação autônoma acontece quando alguma implementação lógica realiza todo o trabalho que seria realizado por ações humanas. A implementação lógica costuma ser realizada através de algoritmos. Neste post será apresentado a navegação autônoma usando algoritmo Dijkstra no robô Turtlebot3 Waffle Pi.


### Um pouco sobre o Turtlebot 3

{:.center}
[![drawing550](../assets/img/2021-12-20-turtlebot-dijkstra/turtlebot.png)](../assets/img/2021-12-20-turtlebot-dijkstra/turtlebot.png)

O Turtlebot 3 Waffle Pi é um robô desenvolvido pela Robotis. É um robô de
pequeno porte, projetado para operar em locais internos
para fins educacionais. O sistema de sensoriamento do Turtlebot 3 possui uma Raspberry Pi camera, lidar, imu e dois encoders. A atuação é desempenhada por dois servomotores. O robô também tem uma placa de processamento Raspberry, que é responsável pelos processamento da maioria dos algoritmos do robô. O Turtlebot 3 é desenvolvido para operar usando ROS, o que possibilita  a implementação de diversas  funcionalidades. O ROS detêm o pacote de software [move_base](http://wiki.ros.org/move_base) que permite a implementação da navegação autônoma de robôs diferenciais. O pacote move_base usa o algoritmo Dijkstra como padrão, mas outras lógicas podem ser implementadas. 

### Um pouco sobre o Algoritmo Dijkstra
 
o algoritmo Dijkstra é capaz de obter uma trajetória entre
dois nós. Esses dois nós podem ser vistos como pontos distintos no ambiente. De um certo nó no
espaço, o algoritmo Dijkstra obtem a partir de todos nós disponíveis uma trajetória para o outro nó, o objetivo. Os gifs abaixo apresentam a aplicação desta técnica desenvolvida em Python por [Atsushi Sakai](https://iopscience.iop.org/article/10.1088/1757-899X/705/1/012037/pdf). A parte em azul são os nós, locais no ambiente, que já
foram explorados. É possível observar que a uma região em azul aumenta à medida que procura pela trajetória continua. Quando o ponto final, o objetivo, é encontrado, temos o trajeto a ser percorrido pelo robô.

{:.center}
[![drawing550](../assets/img/2021-12-20-turtlebot-dijkstra/dij1.gif)](../assets/img/2021-12-20-turtlebot-dijkstra/dij1.gif)

<br>

{:.center}
[![drawing550](../assets/img/2021-12-20-turtlebot-dijkstra/dij2.gif)](../assets/img/2021-12-20-turtlebot-dijkstra/dij2.gif)
 


### Navegação
 
Agora  que o Turtlebot 3 e e o algoritmo Dijkstra já foram citados. Podemos falar da navegação que foi implementada. A aplicação foi realizada em dois tipos de ambientes: simulado e real. Na simulação, o robô inicialmente não conhecia o mapa. Para adquirir dados do mapa foi utilizda a técnica SLAM que permite a geração de mapa do ambiente e localização do veículo ao mesmo tempo. Um exemplo da aplicação de SLAM é demonstrado no projeto [APEREA](https://mhar-vell.github.io/rasc/2021-07-28-aperea-slam/).
 
No ambiente real configuração, o robô inicia a execução da exploração com o conhecimento do mapa. Nesta configuração é usada a técnica AMCL que permite a localização do robô usando os dados do mapa.


### Resultados
 
Na simulação e com auxílio do SLAM, o Turtlebot teve sucesso ao alcançar o objetivo. Vale considerar que nesta aplicação o robô não tem, inicialmente, nenhum conhecimento do ambiente.
 
 
No ambiente real e com auxílio da aplicação do AMCL, o robô também teve sucesso com a exploração. O Turtlebot enfrentou algumas dificuldades ao contornar os obstáculos.
 
{:.center}
[![drawing550](../assets/img/2021-12-20-turtlebot-dijkstra/turtle_waffle.gif)](../assets/img/2021-12-20-turtlebot-dijkstra/turtle_waffle.gif)
 
 
Com o AMCL, o robô teve sucesso quanto a navegação  no ambiente real, apesar de enfrentar dificuldades ao contornar as extremidades das paredes. As dificuldades para passar pelas extremidades podem ser vencidas os parâmetros dedicados à trajetória para evitar obstáculos.
 
{:.center}
[![drawing550](../assets/img/2021-12-20-turtlebot-dijkstra/real_waffle.gif)](../assets/img/2021-12-20-turtlebot-dijkstra/real_waffle.gif)
 
 
A aplicação da navegação autônoma no Turtlebot 3 Waffle Pi foi bastante interessante já que esta funcionalidade é bastante importante para a robótica móvel. Também vale notar que este algoritmo pode ser utilizados em UGV de médio e grande porte com sucesso. 


<br>


---------------------
<br>

<!-- autor -->
<center><h3 class="post-title">Autor</h3><br/></center>
<div class="row">
  <div class="col-xl-auto offset-xl-0 col-lg-4 offset-lg-0 center">
    <table class="table-borderless highlight">
      <thead>
        <tr>
          <th><img src="{{ 'assets/img/people/matheusanselmo-1.png' | relative_url }}" width="100" alt="matheusanselmo" class="img-fluid rounded-circle" /></th>
        </tr>
      </thead>
      <tbody>
        <tr class="font-weight-bolder" style="text-align: center margin-top: 0">
          <td>Matheus Anselmo</td>
        </tr>
        <tr style="text-align: center" >
          <td style="vertical-align: top"><small>Pesquisador Jr. do projeto <br>Engenheiro de Controle e Automação.</small></td>
          <td></td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<br>






