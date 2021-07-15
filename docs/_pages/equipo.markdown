---
layout: page
title: Equipo
permalink: /equipo/
---

<ul>
{% for org_hash in site.data.orgs %}
{% assign org = org_hash[1] %}
{% if org.members %}
    {% for member in org.members %}
    {% if member.name %}
    <h2 style="float: center;">{{ member.name }}</h2>
    <p style="float: right; border: 10px #ddd; border-radius: 3px; padding: 20px;"><img src="{{ member.image }}" height="150px" width="150px"></p>
        <p><strong>Bio</strong>: {{ member.bio }}</p>
        <p><strong>Temas</strong>: {{ member.topics }}</p>
        <p><strong>Correo-e</strong>: <a href="mailto:{{ member.e-mail }}">{{ member.e-mail }}</a></p>
    {% for link in member.links %}
    {% if member.links %}
    <li><a href="{{ link.link }}">{{ link.link }}</a></li>
    {% endif %}
    {% endfor %}
    {% endif %}
    {% endfor %}
{% endif %}
{% endfor %}
<ul>


<!-- <div>
<div style="clear: right;">
{% for member in site.data.members %}
    {% if member.nombre contains "Mario" %}
    <p>Nombre: {{ member.nombre }}<p>
    <p style="float: right;"><img src="{{ member.imagen }}" height="110px" width="110px" border="2px"></p>
    <p>Bio: {{ member.bio }}</p>
    <p>Temas: {{ member.temas }}<p>
    <p>Correo-e: {{ member.correo }}</p>
    <p>{{ member.enlaces }}<p>
    {% endif %}
{% endfor %}

{% for member in site.data.members %}
    {% if member.nombre contains "Francisca" %}
    <p>Nombre: {{ member.nombre }}<p>
    <p style="float: right;"><img src="{{ member.imagen }}" height="110px" width="110px" border="2px"></p>
    <p>Bio: {{ member.bio }}</p>
    <p>Temas: {{ member.temas }}<p>
    <p>Correo-e: {{ member.correo }}</p>
    {{ member.enlaces }}   
    {% endif %}
{% endfor %}

{% for member in site.data.members %}
    {% if member.nombre contains "Roberto" %}
    <p>Nombre: {{ member.nombre }}<p>
    <p style="float: right;"><img src="{{ member.imagen }}" height="110px" width="110px" border="2px"></p>
    <p>Bio: {{ member.bio }}</p>
    <p>Temas: {{ member.temas }}<p>
    <p>Correo-e: {{ member.correo }}</p>

<ul>
{% for enlace_hash in site.data.members %}
{% assign enlace = enlaces_hash[1] %}
  <li>
    <a href={{ enlace.enlaces | size }} enlaces>
    </a>
  </li>
{% endfor %}
</ul>


    {% endif %}
{% endfor %}
<div> -->
