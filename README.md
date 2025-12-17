# Cafeteria-Delicioso
Es una cafetería
# ☕ Cafetería Delicioso - Sistema de Gestión Web

Sistema web completo para la gestión de una cafetería, incluyendo panel administrativo para productos/ventas y una interfaz pública para clientes con carrito de compras y generación de boletas electrónicas en PDF.

## 🚀 Características

### 👥 Parte Pública (Clientes)
- **Catálogo de Productos**: Visualización de menú con imágenes y precios.
- **Filtros y Búsqueda**: Filtrado por categorías (Cafés, Postres, etc.) y barra de búsqueda en tiempo real.
- **Carrito de Compras**: Agregar productos, ver resumen y calcular total.
- **Generación de Boleta**: Emisión automática de boleta en PDF (formato ticket 80mm) con código QR.
- **Diseño Responsive**: Adaptable a móviles y computadoras.

### 🛡️ Panel Administrativo
- **Dashboard (KPIs)**: Estadísticas en tiempo real de ventas (diarias, mensuales), ticket promedio y productos top.
- **Gestión de Productos**: CRUD completo (Crear, Editar, Eliminar) con subida de imágenes y categorías.
- **Gestión de Categorías**: Administrar las categorías del menú.
- **Gestión de Pedidos**: Ver historial de ventas, estado (completado/cancelado) y detalles.
- **Gestión de Usuarios**: Administrar usuarios y roles (admin/cliente).
- **Seguridad**: Login con sesiones, contraseñas encriptadas (bcrypt) y protección básica.

## 🛠️ Tecnologías Utilizadas

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla), Bootstrap 5.
- **Backend**: PHP 8.0+
- **Base de Datos**: MySQL / MariaDB.
- **Librerías Extra**: 
  - `FPDF` (Generación de PDF)
  - `phpqrcode` (Generación de códigos QR)

## 📦 Instalación

1. **Requisitos**:
   - Tener instalado **XAMPP** o similar (Apache + MySQL/MariaDB).

2. **Copiar Archivos**:
   - Descarga el código y por la carpeta `cafeteria` dentro de `C:\xampp\htdocs\`.
   - La ruta final debe ser: `C:\xampp\htdocs\cafeteria`.

3. **Base de Datos**:
   - Abre **phpMyAdmin** (`http://localhost/phpmyadmin`).
   - Crea una nueva base de datos llamada `cafeteria`.
   - Importa el archivo `database_completa.sql` (ubicado en la raíz del proyecto).
   - *Este archivo creará todas las tablas necesarias y el usuario administrador por defecto.*

4. **Configuración (Opcional)**:
   - Si tu contraseña de root en MySQL no es vacía, edita el archivo `db.php` con tus credenciales.

## 🔑 Credenciales de Acceso

### Usuario Administrador
- **Email**: `admin@cafeteria.com`
- **Contraseña**: `admin123`

## 🖥️ Cómo usar

1. **Iniciar el servidor**: Abre el panel de control de XAMPP e inicia "Apache" y "MySQL".
2. **Acceder a la web**:
   - **Pública**: Ir a [http://localhost/cafeteria](http://localhost/cafeteria)
   - **Admin**: Ir a [http://localhost/cafeteria/login.php](http://localhost/cafeteria/login.php) e ingresar con las credenciales de arriba.

## 📄 Estructura de Directorios

- `admin/`: Archivos del panel de control.
- `backend/`: Lógica de negocio (generar boleta, procesar ventas).
- `boletas/`: Directorio donde se guardan los PDFs generados.
- `uploads/`: Imágenes de productos y avatares.
- `fpdf/` & `phpqrcode/`: Librerías de terceros.
- `index.php`: Página principal.
- `productos.php`: Catálogo filtrable.

---
*Desarrollado para el Proyecto Final de Desarrollo Web.*

