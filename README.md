# Tooltip UI Component

Un componente de **tooltips accesibles y responsivos** creado con **HTML y CSS puro**. Permite mostrar mensajes contextuales al pasar el mouse sobre elementos de navegación u otros componentes de la interfaz, sin necesidad de JavaScript.

[![Project](https://roadmap.sh/projects/tooltip-ui)](https://roadmap.sh/projects/tooltip-ui)

---

## 🎯 Características

- Tooltips creados con pseudo-elementos (`::before` y `::after`)
- Diseño minimalista y accesible
- Animaciones suaves con transición `fade`
- Construido sin dependencias externas ni JavaScript
- Fácil de personalizar (texto, color, posición)
- Compatible con todos los navegadores modernos

---

## 🚀 Cómo usar

1. Cloná este repositorio o descargá el archivo `.zip`.
2. Abrí `index.html` en tu navegador para ver el tooltip en acción.
3. Editá los elementos con la clase `.tooltip` y el atributo `data-title` para personalizar el contenido del tooltip.
4. Modificá `style.css` para cambiar colores, posición o animaciones.

---

## 🔧 Personalización

- **Texto del tooltip**: definido con el atributo `data-title` en el elemento HTML.
- **Colores y estilos**: controlados desde `style.css` (`background`, `color`, `padding`, etc.).
- **Transición**: ajustá la duración y efecto en la clase `.tooltip.fade`.
- **Posición**: actualmente el tooltip aparece debajo del elemento, pero se puede ajustar con las propiedades `top`, `left` y `transform`.

---

## 📁 Estructura del Proyecto

```
Tooltip-UI/
├── index.html               # Estructura HTML con tooltips de ejemplo
├── style.css                # Estilos CSS para los tooltips
├── assets/
│   └── preview.png          # Imagen opcional de vista previa
└── README.md                # Este archivo
```

---

## 🧪 Ejemplo de implementación

```html
<li class="tooltip fade" data-title="Here you come to the home">Home</li>
```

```css
.tooltip:before {
  background: rgba(0, 0, 0, 0.75);
  color: #fff;
  content: attr(data-title);
  font-size: 14px;
  padding: 6px 10px;
  top: 26px;
  white-space: nowrap;
}
```

---

## 📸 Captura de pantalla

> Podés agregar una imagen en `assets/preview.png` para mostrar cómo lucen los tooltips en acción.

---

## 📜 Licencia

Este proyecto está bajo la **Licencia Apache-2.0**. Podés usarlo, modificarlo y distribuirlo libremente bajo sus términos.

---

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Podés abrir un `issue` o enviar un `pull request` para:

- Mejorar la accesibilidad de los tooltips
- Agregar posiciones configurables (arriba, abajo, izquierda, derecha)
- Añadir animaciones más complejas
- Explorar una versión con soporte de JavaScript

---

Hecho con ❤️ por [David Rogaci](https://github.com/davidrogaci)
