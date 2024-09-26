---
title: Presentation 2
layout: post
permalink: /presentation-2/

slides:
  - title: Sensores Ópticos
    slide-data: |
      1.1.1 **Tipos**: <br>
      - Fotoeléctricos <br>
      - Infrarrojos <br>
      - LIDAR <br>
      - Cámaras Ópticas
    background: "#e74c3c"

  - title: Sensores Ópticos (Cont.)
    slide-data: |
      1.1.2 **Funcionamiento**: <br>
      Emisión y recepción de luz para detectar cambios en el entorno. Se usa un haz de luz que puede interrumpirse o reflejarse por un objeto.
    background: "#e74c3c"

  - title: Sensores Ópticos (Cont.)
    slide-data: |
      1.1.3 **Características**: <br>
      - Alta precisión <br>
      - Respuesta rápida <br>
      - Sensibilidad a la luz ambiental o polvo
    background: "#e74c3c"

  - title: Sensores Ópticos (Cont.)
    slide-data: |
      1.1.4 **Modo de comunicación**: <br>
      - Señales analógicas/digitales <br>
      - I2C <br>
      - SPI
    background: "#e74c3c"

  - title: Sensores de Temperatura
    slide-data: |
      1.2.1 **Tipos**: <br>
      - Termopares <br>
      - Termistores <br>
      - RTD <br>
      - Sensores IR
    background: '#f1c40f'

  - title: Sensores de Temperatura (Cont.)
    slide-data: |
      1.2.2 **Funcionamiento**: <br>
      Miden la temperatura mediante la variación de resistencia, voltaje o detección de radiación infrarroja.
    background: '#f1c40f'

  - title: Sensores de Temperatura (Cont.)
    slide-data: |
      1.2.3 **Características**: <br>
      - Alta precisión (especialmente RTD) <br>
      - Amplio rango de medición <br>
      - Tamaño compacto
    background: '#f1c40f'

  - title: Sensores de Temperatura (Cont.)
    slide-data: |
      1.2.4 **Modo de comunicación**: <br>
      - Señales analógicas/digitales <br>
      - I2C <br>
      - SPI <br>
      - 1-Wire
    background: '#f1c40f'

  - title: Sensores de Presión
    slide-data: |
      1.3.1 **Tipos**: <br>
      - Piezoeléctricos <br>
      - Capacitivos <br>
      - Resistivos
    background: '#9b59b6'

  - title: Sensores de Presión (Cont.)
    slide-data: |
      1.3.2 **Funcionamiento**: <br>
      Detectan la presión a través de la deformación de materiales que generan una señal eléctrica.
    background: '#9b59b6'

  - title: Sensores de Presión (Cont.)
    slide-data: |
      1.3.3 **Características**: <br>
      - Alta durabilidad <br>
      - Rango de presión amplio <br>
      - Robustos y resistentes
    background: '#9b59b6'

  - title: Sensores de Presión (Cont.)
    slide-data: |
      1.3.4 **Modo de comunicación**: <br>
      - Señales analógicas/digitales <br>
      - I2C <br>
      - SPI <br>
      - CAN bus
    background: '#9b59b6'

  - title: Sensores de Proximidad
    slide-data: |
      1.4.1 **Tipos**: <br>
      - Inductivos <br>
      - Capacitivos <br>
      - Ultrasónicos <br>
      - Ópticos
    background: '#3498db'

  - title: Sensores de Proximidad (Cont.)
    slide-data: |
      1.4.2 **Funcionamiento**: <br>
      Detección de proximidad mediante cambios en campos electromagnéticos, capacitancia, ondas sonoras o luz.
    background: '#3498db'

  - title: Sensores de Proximidad (Cont.)
    slide-data: |
      1.4.3 **Características**: <br>
      - Alta precisión <br>
      - Rango de detección variable <br>
      - Resistencia a condiciones ambientales adversas (polvo, agua)
    background: '#3498db'

  - title: Sensores de Proximidad (Cont.)
    slide-data: |
      1.4.4 **Modo de comunicación**: <br>
      - Salidas digitales o analógicas <br>
      - Protocolos: I2C, SPI, RS-232, RS-485
    background: '#3498db'


{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1><p>{{ slide.slide-data | newline_to_br }}</p></section>
                    
{% endfor %}
