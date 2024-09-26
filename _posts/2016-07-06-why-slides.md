---
title: Tipos de Actuadores
layout: post
permalink: /actuadores/
background: '#0a5'

slides:
  - title: "Información del Estudiante"
    slide-data: |
      <p><strong>Alumno:</strong> Brian Enrique Leal Fuerte</p>
      <p><strong>Profesor:</strong> Dr. Ismaes Jiménez Sánchez</p>
      <p><strong>Materia:</strong> Sistemas Programables</p>
      <p><strong>Tarea:</strong> Presentación de la Unidad 1</p>
      <p><strong>Carrera:</strong> Ingeniería en Sistemas</p>
      <p><strong>Grado:</strong> Noveno Semestre</p>
  
  - title: "Actuadores: Introducción"
    slide-data: |
      <p>Los actuadores son dispositivos que convierten energía en movimiento. Son clave en sistemas de automatización, robótica y maquinaria industrial.</p>
  
  - title: "Actuadores Eléctricos"
    slide-data: |
      <ul>
        <li>Funcionan con energía eléctrica.</li>
        <li>Convierten electricidad en movimiento mecánico.</li>
        <li>Ejemplos: Motores eléctricos, solenoides.</li>
        <li>Ventajas: Precisión, control remoto.</li>
      </ul>
    background: "#e74c3c"

  - title: "Actuadores Mecánicos"
    slide-data: |
      <ul>
        <li>Basados en sistemas mecánicos como palancas, engranajes, o resortes.</li>
        <li>Transforman energía en movimiento mediante mecanismos físicos.</li>
        <li>Ejemplos: Actuadores de leva, tornillo de bola.</li>
        <li>Ventajas: Simplicidad y durabilidad.</li>
      </ul>
    background: "#f1c40f"

  - title: "Actuadores Hidráulicos"
    slide-data: |
      <ul>
        <li>Funcionan con fluidos bajo presión (aceite o agua).</li>
        <li>Convierten energía hidráulica en movimiento.</li>
        <li>Ejemplos: Cilindros hidráulicos, motores hidráulicos.</li>
        <li>Ventajas: Fuerza y potencia elevada.</li>
      </ul>
    background: "#2ecc71"

  - title: "Comparación"
    slide-data: |
      <table>
        <thead>
          <tr>
            <th>Tipo</th>
            <th>Ventajas</th>
            <th>Desventajas</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Eléctrico</td>
            <td>Precisión, fácil control</td>
            <td>Menos potencia que hidráulico</td>
          </tr>
          <tr>
            <td>Mecánico</td>
            <td>Simplicidad, confiabilidad</td>
            <td>Requiere mantenimiento físico</td>
          </tr>
          <tr>
            <td>Hidráulico</td>
            <td>Alta fuerza</td>
            <td>Fugas y mantenimiento</td>
          </tr>
        </tbody>
      </table>
    background: "#9b59b6"

  - title: "Conclusión"
    slide-data: |
      <p>La elección del actuador depende de la aplicación: para precisión, los eléctricos son ideales; para fuerza, los hidráulicos son más adecuados; y para simplicidad, los mecánicos ofrecen durabilidad.</p>
    background: "#34495e"
---

{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
        <h1>{{slide.title}}</h1>{{ slide.slide-data }}
</section>               
{% endfor %}

