# Proyecto: Componentes de UI para Resumen Clínico

Este repositorio contiene la implementación de un conjunto de componentes de UI (widgets) para un panel de resumen clínico. El objetivo es proporcionar a los médicos una vista rápida, interactiva y organizada de la información clave de un paciente, basada en la siguiente historia de usuario.

## 📸 Demo Visual

![Screenshot de la aplicación](./preview/screenshot.png)


## ✨ Características Principales

El proyecto se centra en desarrollar cinco componentes modulares:

1.  **`AgregarDatoSalud`**: Un widget interactivo con navegación por pestañas (`TODOS`, `DIAGNÓSTICO CIE-10`, `HALLAZGOS CLÍNICOS`) que permite al usuario iniciar flujos para añadir nueva información.
2.  **`HistorialClinico`**: Muestra una lista dinámica de eventos clínicos pasados.
3.  **`TratamientoActual`**: Despliega la lista de medicamentos que el paciente está tomando actualmente.
4.  **`Plan`**: Visualiza el plan de tratamiento prescrito a futuro.
5.  **`Paraclinicos`**: Presenta resultados de laboratorio, con indicadores de alerta para valores fuera de rango.

Todos los componentes de visualización de datos están diseñados para ser **dinámicos**, renderizando su contenido a partir de una lista de datos (array) proporcionada.

## 💻 Pila Tecnológica (Tech Stack)

*   **Framework de Frontend:** [Ej: React, Vue, Angular, Svelte]
*   **Lenguaje:** [Ej: TypeScript, JavaScript (ES6+)]
*   **Estilos:** [Ej: CSS Modules, Styled-Components, Tailwind CSS, Sass]
*   **Gestor de Paquetes:** [Ej: npm, yarn]

## 🚀 Cómo Empezar

Sigue estos pasos para clonar y ejecutar el proyecto en tu entorno local.

1.  **Clona el repositorio:**
    ```bash
    git clone [URL_DE_TU_REPO.git]
    cd [NOMBRE_DEL_DIRECTORIO]
    ```

2.  **Instala las dependencias:**
    ```bash
    npm install
    ```

3.  **Ejecuta el proyecto en modo de desarrollo:**
    ```bash
    npm start
    ```
    Abre [http://localhost:3000](http://localhost:3000) (o el puerto correspondiente) para verlo en tu navegador.

## 📄 Historia de Usuario Implementada

Para mantener el contexto del desarrollo, aquí está la historia de usuario que guía este proyecto.

<details>
<summary><strong>Ver Historia de Usuario Completa</strong></summary>

### Título: Visualización de Componentes de Resumen Clínico con Contenido Dinámico

**Como** un médico,
**Quiero** visualizar la información clave del paciente organizada en componentes (widgets) que cargan datos dinámicamente y ofrecen opciones de filtrado,
**Para** poder evaluar rápidamente el historial, el plan de tratamiento y los datos relevantes, y así tomar decisiones clínicas más eficientes y seguras.

#### Criterios de Aceptación (AC)

1.  **AC1: Despliegue General de Widgets**: Al cargar, se deben ver los 5 widgets principales.
2.  **AC2: Estructura de Pestañas**: El widget "Agregar dato de salud" debe tener las 3 pestañas.
3.  **AC3: Comportamiento de la Pestaña "TODOS"**: La pestaña "TODOS" debe estar activa por defecto.
4.  **AC4: Comportamiento de Pestañas de Filtro**: Al hacer clic en otras pestañas, el contenido debe actualizarse.
5.  **AC5: Estructura Común de Widgets**: Los widgets de datos deben tener una cabecera, título y un ícono para expandir.
6.  **AC6: Formato de Ítem en "Historial clínico"**: Debe mostrar fecha, descripción y un ícono de ojo.
7.  **AC7: Formato de Ítem en "Tratamiento actual" y "Plan"**: Debe mostrar ícono Rx, medicamento, dosis y posología.
8.  **AC8: Formato de Ítem en "Paraclínicos"**: Debe mostrar ícono, nombre, resultado y opcionalmente alertas.
9.  **AC9: Renderizado de Contenido Dinámico**: Los widgets deben renderizar una lista de ítems a partir de un array de datos, manejando el caso de lista vacía.

</details>