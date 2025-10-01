# Luminax

Luminax es una página web de búsqueda rápida y enfoque educativo. Integra múltiples motores de búsqueda, accesos directos a herramientas clave, filtrado de marcadores y una ventana emergente de consulta con ERNIE X1.1. Todo diseñado para ser ágil, claro y responsive.

---

## Descripción

Luminax facilita:

- Búsquedas instantáneas en el motor que elijas o uno sugerido automáticamente según tu consulta.  
- Acceso directo a traductor, biblioteca digital, imágenes, streaming y mensajería.  
- Importación de tus marcadores en `.html` y filtrado por título o URL.  
- Consulta con ERNIE X1.1 en una ventana emergente que mantiene el foco activo.  

El diseño oscuro y minimalista garantiza comodidad visual y máxima concentración.

---

## Características

- Búsqueda multi-motor (Google, DuckDuckGo, Qwant, Startpage, Mojeek, Dogpile, Metacrawler, Wiby).  
- Selección automática de motor según palabras clave académicas, técnicas o de nicho.  
- Panel de “Enlaces Directos” con botones personalizables.  
- Buscador de marcadores: carga tu archivo, escribe y filtra al instante.  
- Ventana emergente para ERNIE X1.1 con watchdog que recupera el foco.  
- Responsive: adaptado a escritorio y móviles con media queries.  

---

## Instalación

1. Clona o descarga el repositorio:  
   ```bash
   git clone https://github.com/tu-usuario/luminax.git
   ```  
2. Abre `index.html` en tu navegador.  

No requiere servidor ni dependencias externas: todo funciona en el cliente.

---

## Uso

1. Escribe tu consulta en el campo de búsqueda.  
2. Selecciona un motor o deja “Motor automático” para ajustes por palabra clave.  
3. Haz clic en **Buscar**; se abrirá una nueva pestaña con los resultados.  
4. En **Enlaces Directos**, selecciona la herramienta que necesites.  
5. En **Buscador de marcadores**, carga tu archivo `.html` y filtra por texto.  
6. Pulsa **Consultar con ERNIE X1.1** y permite pop-ups para usar el asistente.  

---

## Personalización

- **Motores de búsqueda:** En el bloque JavaScript  
  ```js
  const engines = { /* "clave": "https://...q=" */ };
  ```  
  añade, modifica o elimina pares clave-URL.  
- **Enlaces directos:** Dentro de  
  ```html
  <div class="controls">…</div>
  ```  
  duplica o ajusta botones usando  
  ```html
  <button onclick="window.open('URL','_blank')">Etiqueta</button>
  ```  
- **Estilos:** Modifica el bloque `<style>` para cambiar paleta, tipografía o puntos de quiebre.  

---

## Adaptación móvil

Luminax incorpora:

- `<meta name="viewport" content="width=device-width, initial-scale=1.0">`  
- Flexbox fluido y contenedores con `max-width`.  
- Media query para pantallas ≤ 600 px que organiza elementos en columna.  

Ajusta los valores de `@media` según tus necesidades de diseño.

---

## Estructura del proyecto

```text
luminax/
├─ index.html       # Página principal con todo el código
├─ README.md        # Documentación (este archivo)
└─ assets/          # (opcional) Imágenes o estilos externos
```

---

## Licencia

© 2025 Andrey L Newman. Todos los derechos reservados.

---

## Autor

**Andrey L Newman**  
Desarrollador y diseñador de Luminax.
