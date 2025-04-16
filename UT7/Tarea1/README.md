# Diseño y Animaciones en "Adóptame"

## 🎨 Decisiones de Diseño

- **Enfoque Mobile First**: Se prioriza la legibilidad y usabilidad en dispositivos móviles, usando `flex-direction: column` por defecto y adaptando a `row` en pantallas más grandes.
- **Paleta de Colores**: Se usa un tono marrón (`#835B4D`) como color principal, evocando calidez, tierra y cercanía. El blanco se usa para contraste y limpieza visual.
- **Tipografía**: Se selecciona `'Segoe UI', sans-serif` por su legibilidad y estilo moderno y amigable.
- **Diseño limpio y modular**: El contenido está dividido en secciones claras (`header`, `presentación`, `galería`, `cta`) que facilitan la navegación y comprensión.
- **Uso de SVGs incrustados**: Se utilizan gráficos vectoriales escalables para representar mascotas, permitiendo alta calidad y personalización visual sin pérdida de rendimiento.

## 💫 Animaciones CSS

### `fadeIn`
- **Ubicación**: Se aplica a la galería de mascotas.
- **Función**: Suaviza la aparición del contenido al cargar la sección, generando una transición visual atractiva.
- **Implementación**:
  ```css
  @keyframes fadeIn {
    0% { opacity: 0; transform: translateY(30px); }
    100% { opacity: 1; transform: translateY(0); }
  }