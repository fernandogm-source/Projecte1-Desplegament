# Práctica 1: Sistemas de Control de Versiones

## 1. Introducción Teórica

### ¿Qué es Git?
Git es un sistema de control de versiones distribuido diseñado para rastrear los cambios en el código fuente a lo largo del desarrollo de software. Permite que varios programadores trabajen simultáneamente de forma colaborativa, conservando un historial completo de cambios y facilitando la gestión de diferentes versiones del proyecto.

### ¿Qué es la metodología Git Flow?
Git Flow es un modelo de ramificación (*branching model*) para Git que define una estructura estricta de ramas organizadas alrededor del ciclo de vida del proyecto. Utiliza principalmente dos ramas estables:
* **`main` / `master`**: Contiene el código de producción listo para la entrega final al cliente.
* **`develop`**: Rama de integración donde se unifican las nuevas características (*features*) en desarrollo.

Y ramas de apoyo temporales:
* **`feature`**: Para el desarrollo de nuevas funcionalidades de forma aislada.
* **`release`**: Para empaquetar y preparar el lanzamiento de una nueva versión.
* **`hotfix`**: Para solucionar errores o aplicar mejoras urgentes directamente sobre producción.

### ¿Por qué la utilizamos en nuestro desarrollo?
Utilizamos Git Flow en este proyecto para mantener una organización profesional del código, evitar conflictos entre los miembros del equipo y asegurar una trazabilidad rigurosa de las versiones entregadas y las correcciones realizadas.

---

## 2. Explicación Detallada del Proceso Realizado

A continuación se detalla el flujo de trabajo llevado a cabo por los 3 programadores del equipo:

### Fase 1: Estructura Inicial (Usuario 1)
El **Usuario 1** (miembro más experimentado) creó el repositorio, inicializó Git Flow y desplegó la estructura base[cite: 2].
* **Acciones:** Configuración del repositorio remoto, creación de las ramas iniciales (`main` y `develop`) y adaptación del boilerplate[cite: 2]. La página incluye la cabecera con el nombre del curso e imagen de fondo, barra de navegación con acceso a Home, descripción central y footer[cite: 1, 2].


### Fase 2: Desarrollo de Contenidos y Atributos (Usuario 2)
El **Usuario 2** desarrolló las secciones dinámicas correspondientes creando dos ramas de tipo *feature*[cite: 2].
* **Acciones:** Creación de `feature/contingutHTML` para añadir ejemplos explicados de modificación de contenido, y `feature/atributsHTML` para la sección de atributos[cite: 1, 2]. Ambas se integraron en `develop`.


### Fase 3: Estilos CSS y Versión Release (Usuario 3)
El **Usuario 3** (integrante nuevo) implementó los estilos visuales de la aplicación[cite: 2].
* **Acciones:** Creación de la rama `feature/estilsCSS` para añadir los estilos y ejemplos comentados[cite: 1, 2]. Posteriormente, creó la rama de lanzamiento (*release*) agrupando todas las características y etiquetándola como **`v1.0`**[cite: 2].


### Fase 4: Pruebas y Mejora mediante Hotfix (Usuario 1)
El **Usuario 1**, encargado de las pruebas del sistema, aplicó una mejora sobre el contenido desarrollado[cite: 2].
* **Acciones:** Creación de la rama de tipo *hotfix* denominada `hotfix/milloresV_1_0` para refinar la sección de contenido HTML[cite: 2]. Tras aplicar los cambios, el hotfix se fusionó con `main` y `develop`.

---

## 3. Gestión del Proyecto y Colaboradores
* **Colaboradores:** Se ha dado acceso como colaborador en el repositorio de GitHub al usuario **`antoni-gimenez`**[cite: 2].
* **Tablero Canvas:** Se ha configurado un proyecto en GitHub tipo Kanban (Canvas) donde figuran registradas todas las *features* y el *hotfix* implementados a lo largo de la práctica con su respectiva información[cite: 2].
