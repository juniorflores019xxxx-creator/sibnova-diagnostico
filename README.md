# Diagnóstico digital · SIBNOVA

Formulario de diagnóstico comercial de **SIBNOVA LTDA. — Soluciones Informáticas de Bolivia**.

En unos 2 minutos, el visitante responde 10 preguntas sobre su negocio y recibe al instante:

- su **nivel de digitalización** (orientativo, de 0 a 100: inicial, en desarrollo o avanzado);
- las **3 soluciones** de SIBNOVA con más impacto para su caso (IA, automatización, integraciones, software de gestión, web o aplicaciones), explicadas con sus propias respuestas;
- un botón para **enviar el diagnóstico por WhatsApp** a SIBNOVA con todas las respuestas ya redactadas.

## Uso

Es una página estática: `index.html` + la carpeta `assets/`. No necesita servidor ni instalación.

- **Abrir en local:** doble clic en `index.html`.
- **Publicar:** GitHub Pages (rama `main`, carpeta raíz) o subir la carpeta a cualquier hosting.

## Personalizar

Todo está en el bloque `<script>` de `index.html`:

| Qué | Dónde |
|---|---|
| Número de WhatsApp que recibe los diagnósticos | `CONFIG.whatsapp` |
| Preguntas y opciones | `STEPS` |
| Textos de las soluciones recomendadas | `SOLUTIONS` |
| Qué respuesta suma puntos a cada solución | `RULES` |
| Cálculo del puntaje y textos de cada nivel | `computeScore` / `levelFor` |
| Google Analytics | bloque comentado en el `<head>` |

## Características

- Una pregunta por pantalla, barra de progreso y avance automático en preguntas de una sola respuesta.
- Atajos de teclado (A, B, C… y Enter) en escritorio; diseño pensado para móvil.
- Las respuestas se guardan en el navegador por si el visitante se interrumpe.
- Accesible: navegación con teclado, foco visible, etiquetas y mensajes de error claros, respeta "reducir movimiento".
- Eventos para Google Analytics / Tag Manager: inicio, cada paso, completado y envío por WhatsApp.

---

© SIBNOVA LTDA. · Santa Cruz de la Sierra, Bolivia · [sibnova.com.bo](https://sibnova.com.bo)
