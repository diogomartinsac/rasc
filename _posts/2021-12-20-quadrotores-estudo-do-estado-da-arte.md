---
layout: post
title: Quadrotores
subtitle: Estudo do Estado da Arte
cover-img: assets/img/quadrotor/dronecrop.jpg
thumbnail-img: assets/img/quadrotor/dronecrop2.jpeg
share-img: /assets/img/rosa-logo-redondo.png
author: Mateus Seixas
comments: true
tags: [blog] #AJUSTAR
---

Quadrotores são aeronaves de asas rotativas, ou seja, são sustentadas e movimentadas
por rotores. Diferente das aeronaves de asas fixas, como aviões, as aeronaves de asas
rotativas não utilizam seu movimento horizontal para sustentar seu vôo. Isso faz com que
esse tipo de veículo apresente um consumo energético muito alto (KARYDIS; KUMAR,
2017). Apesar disso, as aeronaves de asas rotativas apresentam alta manobrabilidadee, possuem a habilidade de realizar pouso e decolagem vertical e também de realizar vôos estacionários ou quase estacionários.

Esses veículos são comumentes chamados de drones, que em inglês significa zangão ou zumbido, pelo barulho gerado pelos seus rotores em sua operação. Os movimentos do quadrotor são obtidos através da combinação das velocidades angulares desses rotores. Para balancear o contra-torque gerado por seus propulsores, é necessário que um par de rotores que estão em uma mesma haste esteja girando no sentido horário, enquanto o outro par de rotores esteja girando no sentido anti-horário.

<center>
  <img src="{{ 'assets/img/sota-quadrotor/800px-Quadcopter_camera_drone_in_flight.jpg' | relative_url }}" width="600" text-align=center alt="img1" />
</center>


## Estudo do Estado da Arte

Foi realizado um documento de estudo do estado da arte para dar suporte no desenvolvimento de um quadrotor autônomo com capacidade de realizar pouso em uma plataforma móvel. Trazendo conhecimento das melhores técnicas que vem sendo utilizadas em áreas como navegação, controle e localização e mapeamento simultâneos (SLAM), assim como os melhores modelos, arquiteturas para conceber um veículo eficiente e principais componentes. A metologia utilizada para o desenvolvimento desse estudo foi o método BILI.

## Método BILI

A pesquisa do estudo do estado da arte desenvolvida neste documento foi elaborada
principalmente a partir do método BILI, que permite realizar uma pesquisa bibliográfica
em um banco de dados de artigos científicos, publicações em periódicos, livros e outras
fontes de conhecimento científicos, fazendo o levantamento das publicações e dos autores
mais impactantes na área pesquisada. Também foram realizadas pesquisas para avaliar as
soluções já encontradas no mercado. O método BILI é dividido em quatro ciclos que acontecem em sequência, como mostrado na Figura 4.3. Eles são chamados de ciclo ingênuo, ciclo otimizada, ciclo de impacto e ciclo de produção, são mais detalhados no documento.

{:.center}
[![drawing500](../assets/img/sota-quadrotor/bili.png)](../assets/img/sota-quadrotor/bili.png) 

## Resultados

Foi feito um estudo do ambiente de desenvolvimento dos quadrotores. Apresentando os tipos de ambiente que os esse tipo de aeronave opera, podendo ser indoor ou outdoor, suas principais aplicações e a situação atual do desenvolvimento, mostrando no que tem se concentrado as principais pesquisas e pesquisadores da área. 

<center>
  <img src="{{ 'assets/img/sota-quadrotor/Package_copter_microdrones_dhl.jpg' | relative_url }}" width="500" text-align=center alt="img1" />
</center>


Foram apresentadas as classificações que existem para esses veículos. Os quadrotores são classificados quanto ao seu peso, podendo ter diferentes categorias dependendo do autor, e também são classificados quanto à disposição dos seus rotores, podendo ter a configuração em "+" ou em "x".

<center>
  <img src="{{ 'assets/img/sota-quadrotor/configs.png' | relative_url }}" width="600" text-align=center alt="img1" />
</center>

Foi feito um estudo dos principais componentes que um quadrotor possui. Os modelos de sensores inerciais, motores, baterias e microcontroladores foram levantados para embasar uma escolha acertada no desenvolvimento de uma plataforma desse tipo.

Por último foi feito o estudo das principais funcionalidades de um quadrotor. Sendo feito o estudo das principais técnicas de controle, falando um pouco de modelagem e identificação do sistema, principais técnicas de planejamento de trajetória e de localização.

## Documento Completo

<br>
<iframe src ="https://drive.google.com/file/d/1Sa2GipjVxa-oJIdlsc7JlCVI1MSaQG1q/preview" width='740' height='430' allowfullscreen mozallowfullscreen webkitallowfullscreen></iframe>
<br>

## Mapa Conceitual

Foi desenvolvido um mapa conceitual para facilitar o entendimento dos conceitos que envolvem esse tipo de plataforma, relacionando eles de uma forma mais visual.

{:.center}
[![drawing500](../assets/img/sota-quadrotor/rovo-seixas-20211026.jpg)](../assets/img/sota-quadrotor/rovo-seixas-20211026.jpg) 

---------------------
<br>

<!-- autor -->
<center><h3 class="post-title">Autor</h3><br/></center>
<div class="row">
  <div class="col-xl-auto offset-xl-0 col-lg-4 offset-lg-0 center">
    <table class="table-borderless highlight">
      <thead>
        <tr>
          <th><img src="{{ 'assets/img/people/mateusseixas-1.png' | relative_url }}" width="100" alt="mateusseixas" class="img-fluid rounded-circle" /></th>
        </tr>
      </thead>
      <tbody>
        <tr class="font-weight-bolder" style="text-align: center margin-top: 0">
          <td>Mateus Seixas</td>
        </tr>
        <tr style="text-align: center" >
          <td style="vertical-align: top"><small>Pesquisador no laboratório de Robótica e Sistemas Autônomos (RoSA), Senai Cimatec, mestrando em Engenharia Elétrica e amante da natuzera.</small></td>
          <td></td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<br>