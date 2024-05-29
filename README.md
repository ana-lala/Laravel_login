# Laravel Login

Este proyecto consiste en una página web de inicio de sesión de usuarios que permite a los usuarios autenticarse de forma segura, crear cuentas, gestionar contraseñas y acceder a su cuenta de usuario. A continuación, se describen las características clave del proyecto, las historias de usuario y los criterios de aceptación.

## Características Principales
- **Autenticación segura**: Los usuarios pueden iniciar sesión utilizando sus credenciales de acceso de manera segura y protegida.
- **Registro de nuevos usuarios**: Permite a los usuarios crear nuevas cuentas proporcionando información básica.
- **Gestión de contraseñas**: Los usuarios pueden restablecer sus contraseñas mediante un proceso de confirmación por correo electrónico.
- **Experiencia de usuario intuitiva**: La interfaz de usuario está diseñada para ser fácil de usar y accesible.
- **Protección de datos**: El proyecto cumple con los estándares de seguridad y privacidad de datos para proteger la información del usuario.

## Historias de Usuario

### Registro de Usuario
1. **Configuración del Entorno de Desarrollo**
   - Configurar un entorno de desarrollo con Laravel para el backend y Blade para el frontend.
   
2. **Esquema de Base de Datos**
   - Crear un esquema de base de datos MySQL para almacenar la información del usuario (nombre, correo electrónico, contraseña, etc.).
   
3. **Backend para Registro de Usuarios**
   - Implementar el backend en Laravel para manejar las solicitudes de registro de usuarios.
   
4. **Formulario de Registro**
   - Crear un formulario de registro en Blade con validación de datos en el servidor utilizando las características de validación de Laravel.
   
5. **Procesamiento de Solicitudes de Registro**
   - Implementar la lógica para procesar la solicitud de registro en el backend, validar datos y almacenar al usuario en la base de datos.
   
6. **Correo Electrónico de Confirmación**
   - Desarrollar la funcionalidad de envío de correo electrónico de confirmación para nuevos usuarios.
   
7. **Pruebas en Contenedores Docker**
   - Probar la aplicación en contenedores Docker para garantizar que funcione correctamente en un entorno aislado y replicable.

### Inicio de Sesión
1. **Interfaz de Usuario de Inicio de Sesión**
   - Crear la interfaz de usuario de la página de inicio de sesión en Blade.
   
2. **Rutas y Controladores de Inicio de Sesión**
   - Configurar las rutas y controladores en el backend para manejar solicitudes de inicio de sesión.
   
3. **Lógica de Autenticación**
   - Implementar la lógica de autenticación en el backend utilizando bcrypt para verificar contraseñas.
   
4. **Establecimiento de Sesión y Token**
   - Establecer la sesión del usuario en el backend después de una autenticación exitosa y devolver un token de acceso JWT al cliente.
   
5. **Cierre de Sesión**
   - Desarrollar la lógica de cierre de sesión para destruir la sesión del usuario y eliminar el token de acceso.

### Gestión de Contraseñas
1. **Solicitud de Restablecimiento de Contraseña**
   - Crear una página en el frontend para que los usuarios soliciten un restablecimiento de contraseña.
   
2. **Generación de Token de Restablecimiento**
   - Implementar la lógica en el backend para generar un token de restablecimiento de contraseña único y enviarlo por correo electrónico al usuario.
   
3. **Verificación del Token**
   - Crear una ruta en el backend para manejar la solicitud de restablecimiento de contraseña y verificar la validez del token.
   
4. **Nueva Contraseña**
   - Desarrollar la interfaz de usuario para que los usuarios ingresen una nueva contraseña después de recibir el correo electrónico de restablecimiento.
   
5. **Actualización de Contraseña**
   - Actualizar la contraseña del usuario en la base de datos después de la confirmación del restablecimiento.

## Criterios de Aceptación
- Todas las funcionalidades de autenticación, registro y gestión de contraseñas deben ser fluidas, sin errores y seguras.
- El sistema debe adherirse a las mejores prácticas para la autenticación y manejo de contraseñas, incluidos cifrado y protección contra amenazas de seguridad comunes.
- Los mensajes y notificaciones al usuario deben ser claros y útiles en todo el proceso.

## Instrucciones para Desarrolladores
### Requisitos Previos
- PHP 7.4 o superior
- Composer
- MySQL
- Node.js (para manejar frontend si es necesario)
- Docker (para pruebas y despliegue)

### Instalación
1. Clonar el repositorio:
   ```bash
   git clone https://github.com/ana-lala/Laravel_login.git
   cd Laravel_login
