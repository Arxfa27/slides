---
title: Presentation 1
layout: post
permalink: /presentation-1/
background: '#0a5'
slides:
 - title: Actuadores Eléctricos - Tipos y Funcionamiento
   slide-data: |
     Tipos: Motores eléctricos, solenoides, actuadores lineales eléctricos, servomotores.<br>
     Funcionamiento: Convierten energía eléctrica en movimiento mecánico.

 - title: Actuadores Eléctricos - Características
   slide-data: |
     Características: Alta precisión, buen rendimiento energético, bajo mantenimiento.

 - title: Actuadores Mecánicos - Tipos y Funcionamiento
   slide-data: |
     Tipos: Levas, cremalleras y piñones, tornillos y tuercas, poleas y correas.<br>
     Funcionamiento: Conversión directa de movimiento en fuerza mediante elementos mecánicos.

 - title: Actuadores Mecánicos - Características
   slide-data: |
     Características: Alta durabilidad, simplicidad, capacidad para soportar cargas pesadas.

 - title: Actuadores Hidráulicos - Tipos y Funcionamiento
   slide-data: |
     Tipos: Cilindros hidráulicos, motores hidráulicos, bombas hidráulicas.<br>
     Funcionamiento: Utilizan la presión de un fluido para generar movimiento.

 - title: Actuadores Hidráulicos - Características
   slide-data: |
     Características: Alta fuerza, precisión moderada, robustez en entornos industriales.

---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
