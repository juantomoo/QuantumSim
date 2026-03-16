# QuantumSim V0.3

Explorador atómico interactivo con tabla periódica completa, vista educativa y visualización 3D de modelos atómicos.

## Estado actual del proyecto

Esta versión quedó configurada para ejecutarse **en local sin instalar Node.js, Vite ni React por npm**.

La app funciona como una SPA estática usando:

- `React` por CDN
- `ReactDOM` por CDN
- `Babel Standalone` para interpretar JSX en el navegador
- `Tailwind CSS` por CDN
- `Three.js` cargado dinámicamente para la simulación 3D

Eso la hace ideal para abrirla rápido, probarla localmente y moverla entre carpetas sin build previo.

## Archivo principal

- [index.html](index.html): aplicación completa lista para abrir en navegador.

## Cómo ejecutarlo en local

### Opción recomendada: servidor local simple

Desde esta carpeta, inicia un servidor local. Por ejemplo:

- con Python: `python3 -m http.server 8080`

Luego abre en tu navegador:

- `http://localhost:8080`

### Opción rápida

También puedes abrir [index.html](index.html) directamente en el navegador, pero un servidor local suele evitar problemas de compatibilidad y caché.

## Funcionalidades incluidas

- Tabla periódica de los 118 elementos
- Búsqueda por nombre, símbolo y número atómico
- Filtros por categoría, bloque y estado
- Modo estudio
- Vista educativa de fundamentos
- Modal de detalle por elemento
- Visualización 3D:
  - Modelo de Bohr
  - Modelo cuántico
- Interacción con ratón:
  - arrastre para rotar
  - rueda para zoom
- Interfaz bilingüe:
  - Español
  - English

## Datos integrados

La base de datos de elementos contiene:

- número atómico
- símbolo
- nombre en español e inglés
- masa atómica
- categoría
- bloque
- estado
- configuración electrónica
- electronegatividad
- grupo y período
- descripción extendida en ambos idiomas

## Notas técnicas

- `Three.js` se carga dinámicamente desde CDN cuando se necesita el visor.
- Las fuentes web también se cargan automáticamente.
- Los iconos fueron adaptados para funcionar sin dependencias externas de build.
- Esta versión está pensada como **entrega portable** y no como proyecto con bundler.

## Si luego quieres migrarlo a Vite

Se puede hacer sin problema:

1. crear un proyecto con Vite
2. mover la lógica a `src/App.jsx`
3. separar datos, componentes y estilos
4. instalar dependencias reales por npm

Pero para usarlo localmente **ya no hace falta hacer eso**.

## Autoría

- Desarrollado por JuanTomoo
- Licencia MIT
