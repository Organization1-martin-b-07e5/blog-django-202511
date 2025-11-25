ÚLTIMA ACTUALIZACIÓN 25-11-2025 (VERSIÓN BORRADOR)

Este repositorio contiene el código fuente para el Proyecto Final - ETAPA 2 del Informatorio Chaco, consistente en una aplicación web tipo **Blog** desarrollada con **Django** y base de datos, orientada a la promoción de noticias y artículos.


| Categoría | Tecnología | Versión Clave |
| :--- | :--- | :--- |
| **Backend/Framework** | Python / Django |
| **Base de Datos** | *******COMPLETAR....*******
| **Frontend** | HTML5, CSS3, JavaScript
| **Estilos/Framework CSS**| *******COMPLETAR....*******
| **Control de Versiones** | Git / GitHub | N/A |
| **Despliegue (Deploy)** | PythonAnywhere | N/A |



## ⚙️ Funcionalidades Mínimas

La versión mínima del proyecto incluye las siguientes características:

### 1. Sistema de Usuarios y Autenticación
* **Perfiles:** Gestión de acceso para perfiles **`admin`** (administrador) y **`registrado`** (usuario estándar).
* **Login:** Funcionalidad de inicio de sesión para ambos tipos de usuarios.

### 2. Gestión de Contenido (Posts)
* **Creación:** Carga de nuevos posts (solo para usuarios con permisos específicos, típicamente `admin`).
* **Eliminación:** Eliminación de posts publicados (con restricciones según el perfil de usuario).

### 3. Interacción
* **Comentarios:** Los usuarios con perfil **`registrado`** y **autenticados** pueden comentar en los posts.

### 4. Búsqueda y Navegación
* **Filtrado de Posts:** Posibilidad de buscar y ordenar posts por:
    * **Fecha de publicación**
    * **Categoría**
    * **Cantidad de comentarios recibidos**


FASES DEL PROYECTO:

1. Planificación y Configuración
2. Backend y Base de Datos
3. Frontend y Lógica Avanzada
4. Pruebas, Documentación y Entrega





FASE 1:
1.1	Definición de Alcance

Requisito Mínimo	Permisos/Restricciones Clave
Gestión de Cuentas	Login y Registro para perfiles admin y registrado.
Creación de Posts	Solo usuarios con perfil admin pueden crear nuevos posts.
Eliminación de Posts	Solo usuarios con perfil admin pueden eliminar posts.
Comentarios	        Solo usuarios con perfil registrado (y autenticados) pueden comentar.
Sistema de Filtros	Filtros visibles para todos los usuarios por Fecha, Categoría y Comentarios recibidos.


1.2	Diseño de Modelos (Clases) en "models.py"

Diseñar la estructura de la base de datos. Se sugiere 4 modelos:

	Modelos de Usuarios y Perfiles
	Modelos de categorías (esto va a permitir filtrar los posteos)
	Modelos de Post (título, categoría, contenido, fecha de publicación, autor...) 
	Modelo de Comentarios (Post al que pertenece, contenido, fecha de publicación, autor...)

Definir las relaciones entre los Modelos:

Post (1:N) con Usuario

Post (N:M) con Categoría

Post (1:N) con Comentario


  


1.3	Configuración Inicial del Entorno
1.4	Configuración de GitHub
1.5	Diseño del Layout (Wireframes)
2.1	Implementación de Modelos
2.2	Migraciones Iniciales
2.3	Configuración de Administración
2.4	Sistema de Perfiles y Autenticación
2.5	CRUD Básico de Posts
3.1	Maquetación de Plantillas Base
3.2	Desarrollo de Comentarios
3.3	Implementación de Filtros
3.4	Restricciones de Permisos
4.1	Revisión de Funcionalidades
4.2	Ajuste de Estilos
4.3	Creación de requirements.txt
4.4	Preparación de la Documentación
4.5	Despliegue Final (PythonAnywhere)
4.6	Entrega
