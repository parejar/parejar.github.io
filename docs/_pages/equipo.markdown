---
layout: page
title: Equipo
permalink: /equipo/
---

<div>
<div style="clear: right;">
    <p style="float: right;"><img src="\assets\images\mario-foto-perfil.jpg" height="110px" width="110px" border="2px"></p>
    <p>Mario Portugal-Ramírez es sociólogo por la Universidad Autónoma Gabriel René Moreno (Bolivia), magíster en sociología por la Facultad Latinoamericana de Ciencias Sociales (FLACSO) Ecuador y candidato a doctor por la Universidad de Massachusetts Boston. Sus temas de investigación son salud digital y salud global. En la actualidad investiga sobre la implementación de Records Médicos Electrónicos en los sistemas de salud.</p>
<ul>
{% for member in site.data.members %}
    {% if member.name contains "Mario" %}
  <li>
    <p>
      {{ member.email }}
    </p>        
  </li>
    {% endif %}
{% endfor %}
</ul>
</div>
<div style="clear: right;">
    <p style="float: right;"><img src="\assets\images\francisca-foto-perfil.png" height="110px" width="110px" border="2px"></p>
    <p>Francisca Gomez-Baeza es psicóloga por la Universidad de Chile, magíster en políticas públicas por la Facultad de Economía de la misma universidad, magíster en sociología por la Universidad de Washington Seattle (UW) y estudiante de doctorado en sociología por la misma universidad. Sus temas de investigación son criminalización y tecnologías de control social. Actualmente investiga los orígenes, transformaciones y usos de datos en el sistema de justicia criminal.</p>
<ul>
{% for member in site.data.members %}
    {% if member.name contains "Francisca" %}
  <li>
    <p>
      {{ member.email }}
    </p>
  </li>
    {% endif %}
{% endfor %}
</ul>
</div>
<div style="clear: right;">
    <p style="float: right;"><img src="\assets\images\roberto-foto-perfil.bmp" height="110px" width="110px" border="2px"></p>
    <p>Roberto Pareja es doctor en Literatura Latinoamericana y Estudios Culturales por la Universidad de Georgetown en Washington DC, Estados Unidos, y magíster en Information Studies por la Universidad de McGill en Montreal, Canadá. Su trabajo como investigador en las Humanidades y Humanidades Digitales se concentra en la historia intelectual y el estudio de las redes de actores en la conformación de mediaciones político-culturales en América Latina desde una perspectiva global. Forma parte del proyecto de historia social <a href="https://limandina.org/">Lima Andina</a> en Toronto y del colectivo interinstitucional <a href="https://www.projet-medetlat.com/">Médiation éditoriale, diffusion et traduction de la littérature latino-américaine en France, de 1945 à 2000 (MEDET-LAT)</a> en París, para los cuales diseñó las bases de datos. Actualmente sigue colaborando tanto con Lima Andina como con MEDET-LAT en la implementación de un interfaz de búsqueda con múltiples criterios dirigido a un público tanto académico como general para dar acceso a los datos del proyecto. Su trabajo más reciente estudia la mediación editorial de la literatura boliviana a nivel global usando datos de diversos repositorios.</p>
<ul>
{% for member in site.data.members %}
    {% if member.name contains "Roberto" %}
  <li>
    <p>
      {{ member.email }}
    </p>
  </li>
    {% endif %}
{% endfor %}
{% for member in site.data.members %}
    {% if member.link %}
  <li>
    <a href="{{ member.link }}">{{ member.link }}</a>
  </li>
    {% endif %}
{% endfor %}
</ul>
</div>