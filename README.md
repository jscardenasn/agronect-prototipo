# 🌱 AgroNECT Boyacá - Prototipo de Alta Fidelidad

**Universidad Nacional Abierta y a Distancia (UNAD)**
**Curso:** Proyecto de Ingeniería II (Código: 202337121)
**Fase 4:** Componente Práctico - Práctica Simulada
**Grupo Colaborativo:** 101

Este repositorio contiene el código fuente del prototipo web funcional para el proyecto **AgroNECT Boyacá**, una plataforma diseñada para conectar directamente a pequeños y medianos productores agropecuarios de la provincia del Tundama con compradores, eliminando la intermediación comercial.

## 🚀 Acceso al Prototipo en Vivo
Puedes navegar e interactuar con la simulación funcional haciendo clic en el siguiente enlace:
👉 **[Ver AgroNECT Boyacá](https://jscardenasn.github.io/agronect-prototipo/)**

## 🛠️ Tecnologías Utilizadas
*   **HTML5:** Estructura semántica de las vistas.
*   **Tailwind CSS (vía CDN):** Diseño responsivo, moderno y utilitario.
*   **JavaScript (Vanilla):** Lógica de navegación, manipulación dinámica del DOM, filtros de búsqueda, simulación de sesión y persistencia de datos local.
*   **Google Fonts & Material Symbols:** Tipografía y librería de íconos.

## 📱 Funcionalidades del Prototipo (Módulos)
El sistema está compuesto por 4 pantallas interactivas que simulan el flujo real de la plataforma:

1.  **Inicio de Sesión (`index.html`):** Autenticación simulada. El sistema recuerda el nombre del usuario y lo muestra en los paneles internos.
2.  **Catálogo de Productos (`catalogo.html`):** Grid dinámico con buscador en tiempo real, filtros por categoría (frutas, hortalizas, tubérculos) y paginación.
3.  **Detalle del Producto (`detalle.html`):** Recibe los datos del producto seleccionado vía parámetros de URL (nombre, precio, unidad). Incluye gráfico de tendencias y botón de contacto simulado.
4.  **Gestión de Precios - Admin (`admin.html`):** **Núcleo de la Épica 4 (EP04).** Permite registrar nuevos precios de referencia a través de un formulario. Al guardar, el producto se inserta dinámicamente en la tabla de datos y el contador principal (KPI) se actualiza automáticamente. Incluye función para eliminar registros.

## ⚠️ Nota Técnica (Simulación Frontend)
Dado que esta fase del proyecto está enfocada en el prototipado de alta fidelidad (TRL 4), **el sistema no cuenta con un backend ni base de datos relacional en producción**. La simulación de datos se realiza mediante:
*   `localStorage` para la persistencia de la sesión del usuario.
*   `URLSearchParams` para el paso de datos entre el catálogo y el detalle.
*   Arreglos de JavaScript para simular la inserción y eliminación de registros en el panel de administración.

La arquitectura está diseñada y preparada para, en una fase futura, conectarse a un backend real y consumir el WebService oficial del SIPSA (DANE) para la actualización de precios en tiempo real.

## 👥 Autores (Grupo 101)
*   John Sebastián Cárdenas Nova (Product Owner / Desarrollador Frontend)
*   Ronal Santiago Figueredo
*   Diana Mayerly Wilches Soler
*   Carlos Yesid Hernández González

---
*Desarrollado como práctica simulada para el curso de Proyecto de Ingeniería II - UNAD (2026).*
