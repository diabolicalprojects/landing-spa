# 🏨 Documento de Gestión Técnica y Prompt: SpaBooking SaaS Landing

## 1. Contexto del Proyecto
El objetivo es desarrollar una landing page de alta gama para comercializar un sistema de agendamiento automático dirigido a dueños de Spas y centros de estética. La web debe replicar la estética visual de la referencia (WordPress Template), pero con un mensaje enfocado en la venta de software (SaaS) y una llamada a la acción (CTA) orientada a la prueba de una demo.

## 2. Especificaciones Técnicas

| Categoría | Especificación |
| :--- | :--- |
| **Stack Frontend** | React JS (Vite) + TypeScript. |
| **Estilos** | Tailwind CSS. |
| **Arquitectura** | Componentes funcionales, Mobile First. |
| **Diseño / UI** | Basado en el archivo de imagen adjunto (Estética Waxy). |
| **Paleta de Colores** | **Elegant Nude:** Beige (#F5EBE0), Crema (#FAF6F2), Café suave para textos (#604A3E). |
| **Tipografía** | Serif elegante para títulos (estilo Playfair Display) y Sans-serif limpia para cuerpo. |
| **Infraestructura** | VPS con Dokploy (Docker). |
| **Assets Visuales** | Carpeta local `./src/assets/imgs/`. Sustituir fotos de servicios por mockups de software y gestión empresarial. |

---

## 3. Master Prompt para el Agente de IA

*Copia y pega el siguiente texto a tu agente de IA de diseño y desarrollo:*

> **Contexto y Rol:**
> Actúa como un Desarrollador Senior Frontend y Diseñador UI/UX. Tu objetivo es crear una Landing Page profesional para un **Software de Agendamiento para Spas** utilizando **React JS con TypeScript** y **Tailwind CSS**.
>
> **Instrucciones de Diseño (Inspiración en Imagen):**
> 1. **Estética:** Replica fielmente la estructura y elegancia de la plantilla de referencia. Usa bordes redondeados orgánicos (estilo arcos), mucho espacio en blanco y una paleta de colores beige, crema y tierra.
> 2. **Imágenes:** No utilices las imágenes de la plantilla original. Toma las fotos de la carpeta local `./src/assets/imgs/`. Debes priorizar mockups del sistema (laptops/tablets) y fotos de gestión de negocios que encajen en los marcos orgánicos del diseño.
> 3. **Secciones de la Referencia:**
>    - **Hero:** Sustituir "Get The Smooth Look..." por un mensaje B2B: "La gestión de tu Spa, ahora en piloto automático".
>    - **Contadores:** Mantener los contadores visuales para mostrar métricas como 'Citas procesadas', 'Dueños felices' y 'Horas ahorradas'.
>    - **Tarjetas de Servicio:** Convertirlas en **Características del Software**: 1. Agendamiento Online, 2. Recordatorios Automáticos, 3. Control de Inventarios, 4. Reportes Financieros.
>
> **Instrucciones de Desarrollo:**
> 1. Crea la estructura con componentes React limpios y altamente responsivos.
> 2. **CTA (Call to Action):** El botón principal debe decir 'Probar Demo Gratis' o 'Rentar Sistema'. El diseño del botón debe ser minimalista pero con alto contraste.
> 3. Implementa animaciones suaves de entrada (Fade-in) para mantener la sensación de "Spa/Bienestar" en la navegación.
>
> **Entregables:**
> - Código de componentes (.tsx) y configuración de Tailwind.
> - Estructura de `Dockerfile` y `docker-compose.yml` para despliegue en Dokploy.

---

## 4. Gestión de Riesgos y Control de Calidad (PM Notes)

* **Riesgo de Identidad:** Es vital que el usuario entienda que se vende un **sistema**, no servicios de Spa. El copy debe hablar de "Rentabilidad", "Optimización" y "Ahorro de tiempo".
* **Adaptación UI:** La plantilla original usa formas de arco. Asegúrate de que el agente use CSS (Tailwind `rounded-full` con ajustes o `clip-path`) para replicar esos marcos de fotos de manera impecable.
* **Flujo de Demo:** El CTA debe ser el punto focal. Se recomienda un botón "Sticky" en la versión móvil para facilitar el acceso a la demo en cualquier momento del scroll.