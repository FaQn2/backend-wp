# WP Challenge – Backend WordPress

Este repositorio documenta la configuración y contenido del backend utilizado para la prueba técnica. Se utilizó **WordPress** como CMS, montado localmente con **XAMPP**.

---

## 🛠️ Entorno de desarrollo

- Servidor: XAMPP en Windows
- URL local: `http://localhost/wp-challenge`
- WordPress instalado en: `htdocs/wp-challenge`
- Base de datos: `wp_challenge`

---

## 📄 Contenido cargado

### Página para el Banner

- Título: `Inicio`
- Slug: `inicio`
- Imagen destacada
- Contenido: texto + botón 

👉 El frontend consume esta página desde:

/wp-json/wp/v2/pages?slug=inicio



---

### Entradas para la sección de Servicios

- 2 publicaciones creadas
- Categoría: `servicios` (ID: 3)
- Cada post tiene:
  - Título
  - Contenido descriptivo
  - Imagen destacada

👉 Endpoint utilizado:

/wp-json/wp/v2/posts?categories=3


Además, para mostrar las imágenes destacadas, el frontend utiliza:

/wp-json/wp/v2/media/:id


---

## 📷 Capturas

A continuación se muestra una vista del contenido cargado desde el panel de WordPress:

![Admin Screenshot](/cap1.png)
![Admin Screenshot](/cap2.png)
![Admin Screenshot](/cap3.png)
![Admin Screenshot](/cap4.png)

---

## 🧠 Cómo modificar el contenido

1. Acceder al panel:  
   `http://localhost/wp-challenge/wp-admin`

2. **Modificar el banner:**  
   - Ir a “Páginas” > Editar la página `Inicio`
   - Cambiar el título, contenido o imagen destacada

3. **Modificar los servicios:**  
   - Ir a “Entradas” > Agregar/editar publicaciones
   - Asegurarse de asignar la categoría `servicios`
   - Agregar imagen destacada si se desea mostrar

---


