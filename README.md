# 🌿 GreenTech MVP Sostenible

**Desarrollado por:** JESÚS CABEZA CARBALLAR  
**Rol:** Especialista en Sostenibilidad 

## 1. Resumen Ejecutivo
Este proyecto representa la refactorización profunda del Producto Mínimo Viable (MVP) para la campaña "Salvemos el Planeta". El objetivo principal ha sido alinear el desarrollo técnico con el mensaje ecologista de la ONG, eliminando el "bloatware" (dependencias inútiles) que generaba un consumo energético injustificado y sobrecalentamiento en dispositivos de gama baja.

## 2. Auditoría y Decisiones Técnicas
En la versión original, se identificó la importación de frameworks mastodónticos (Bootstrap, jQuery, Moment.js, FontAwesome) para tareas triviales como renderizar un botón o mostrar el año actual. 

**Soluciones implementadas:**
* **CSS Nativo y Vanilla JS:** Se ha prescindido del 100% de las librerías externas. La interfaz es ahora completamente responsiva usando Flexbox y variables CSS nativas, logrando el mismo resultado visual con una fracción del peso.
* **Optimización de Recursos:** La imagen principal de Unsplash se ha redimensionado en la petición HTTP (de `w=3000` a `w=1200`) y se ha implementado el atributo `loading="lazy"`.
* **Sustitución de Iconografía:** Se eliminó la dependencia de FontAwesome integrando un único archivo SVG en línea.
* **Optimización Tipográfica:** Se limitó la petición de Google Fonts estrictamente a los grosores de fuente utilizados (400 y 700).

## 3. Impacto Físico, ASG y Economía Circular
Las decisiones de diseño de software tienen consecuencias físicas tangibles.Al importar dependencias pesadas innecesariamente, estábamos forzando un mayor consumo de ancho de banda y ciclos de CPU, lo que fomentaba la obsolescencia programada al exigir a los usuarios dispositivos más potentes. 

* [cite_start]**Reducción del Carbono Embebido:** Siguiendo las directrices de las *Web Sustainability Guidelines (WSG) 1.0*[cite: 41], al reducir radicalmente el peso de transferencia de la página (eliminando cientos de kilobytes de código muerto), disminuimos la energía requerida por los centros de datos y la red de transmisión.
* [cite_start]**Lucha contra la Obsolescencia Programada:** El enfoque *Green Software* nos enseña que un software eficiente permite que hardware más antiguo siga siendo funcional[cite: 42]. Al aliviar la carga del procesador del cliente final (eliminando jQuery y el repintado excesivo del DOM), alargamos la vida útil de sus baterías y dispositivos, frenando la generación de basura electrónica (e-waste).
* [cite_start]**Ingeniería de Software Verde:** Tal como indican Verdecchia et al., la sostenibilidad técnica (código limpio y mantenible) está intrínsecamente ligada a la sostenibilidad medioambiental en la nube y en el cliente[cite: 43].

## 4. Referencias
[1] W3C, "Web Sustainability Guidelines (WSG) 1.0," World Wide Web Consortium, 2023. [Online]. Available: https://www.w3.org/TR/wsgl/
[2] Green Software Foundation, "Green Software Practitioner Course," 2024. [Online]. Available: https://learn.greensoftware.foundation/
[3] R. Verdecchia, P. Lago, I. Malavolta, y G. Procaccianti, "Green IT and Green Software Engineering: A Systematic Mapping Study," arXiv preprint arXiv:2102.04945, 2021. [Online]. Available: https://arxiv.org/abs/2102.04945
