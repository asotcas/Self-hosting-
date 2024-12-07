# Proyecto AlejandroHosting

Este proyecto configura un servidor web Apache2 para el dominio **alejandrohosting.es**, con varias funcionalidades y requisitos específicos.

## Requerimientos

- **Apache 2.4+**.
- **Certificado SSL**: Let’s Encrypt.
- **Dominio**: alejandrohosting.es.

## Funcionalidades Implementadas

1. **Página de Inicio**
   - Una página de bienvenida que se sirve en `http://alejandrohosting.es/`.

2. **Página de Error 404 Personalizada**
   - Si se accede a una página no existente, se mostrará una página de error personalizada.

3. **Descarga de Imagen**
   - Una imagen se puede descargar desde `http://alejandrohosting.es/logo.png`.

4. **Área de Administración Protegida**
   - La ruta `/admin` requiere autenticación básica con el usuario `admin` y la contraseña `asir`.

5. **Estado del Servidor**
   - La ruta `/server-status` muestra el estado del servidor Apache, accesible solo desde localhost.

6. **Certificado SSL con Let’s Encrypt**
   - Se configura HTTPS con un certificado gratuito de Let’s Encrypt, asegurando la conexión en `https://alejandrohosting.es`.

7. **Pruebas de Rendimiento**
   - Se realizan pruebas de rendimiento usando Apache Bench (`ab`) para evaluar la capacidad del servidor con 100 y 1000 usuarios concurrentes.

## Pasos Realizados

1. **Instalación y Configuración de Apache2**
   - Se instaló Apache y se configuró para escuchar en los puertos HTTP (80) y HTTPS (443).

2. **Creación de la Página de Inicio y Páginas de Error**
   - Se implementó una página de inicio y una página de error 404 personalizada.

3. **Protección de Rutas con Autenticación Básica**
   - Se configuró autenticación para la ruta `/admin`.

4. **Configuración de HTTPS con Let’s Encrypt**
   - Se instaló y configuró un certificado SSL gratuito de Let’s Encrypt para asegurar la comunicación HTTPS.

5. **Habilitación de ModStatus**
   - Se activó el módulo `mod_status` de Apache para mostrar información sobre el estado del servidor.

6. **Pruebas de Carga**
   - Se realizaron pruebas de carga con Apache Bench para medir el rendimiento del servidor.

## Conclusión

El servidor está completamente configurado para servir contenido seguro, proteger rutas administrativas, y ofrecer información sobre su estado. Se recomienda realizar pruebas periódicas de rendimiento y mantener el servidor actualizado.
