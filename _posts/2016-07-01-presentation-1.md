---
title: Presentation 1
layout: post
permalink: /presentation-1/
background: '#0a5'
slides:
 - title: Actuadores Eléctricos
   slide-data: |
     Tipos:<br>
     - Motores eléctricos<br>
     - Solenoides<br>
     - Actuadores lineales eléctricos<br>
     - Servomotores<br><br>

     Funcionamiento:<br>
     Convierten energía eléctrica en movimiento mecánico.

 - title: Actuadores Mecánicos
   slide-data: |
     Tipos:<br>
     - Levas<br>
     - Cremalleras y piñones<br>
     - Tornillos y tuercas<br>
     - Poleas y correas<br><br>

     Funcionamiento:<br>
     Conversión directa de movimiento en fuerza mediante elementos mecánicos.

 - title: Actuadores Hidráulicos
   slide-data: |
     Tipos:<br>
     - Cilindros hidráulicos<br>
     - Motores hidráulicos<br>
     - Bombas hidráulicas<br><br>

     Funcionamiento:<br>
     Utilizan la presión de un fluido para generar movimiento.

---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
