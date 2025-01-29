# Proyecto: Pruebas API Petstore

## Contexto
Este proyecto forma parte de las pruebas funcionales realizadas sobre la API Petstore. El objetivo principal fue validar tres funcionalidades clave de la API: la creación de usuarios, el inicio de sesión de usuarios y la obtención de mascotas por estado. La finalidad de este ejercicio fue familiarizarme con el uso de herramientas de testing como **Postman** y comprender cómo interactuar con APIs para garantizar su correcta implementación y funcionalidad.

## Herramientas Utilizadas
- **Postman**: Herramienta de pruebas de API para realizar solicitudes HTTP y verificar respuestas.
- **Swagger**: Documentación de la API Petstore para conocer las rutas, parámetros y respuestas esperadas.
- **JSON**: Formato de datos utilizado en las respuestas de la API para analizar el contenido de las respuestas.

## Explicación del Proyecto
En este proyecto, me enfoqué en realizar pruebas de tres funcionalidades principales de la API:

1. **Crear un usuario (POST /user)**:
   - Validación de la capacidad de la API para registrar un nuevo usuario.
   - Se realizaron pruebas tanto con datos correctos como con datos faltantes para asegurar que la API maneja correctamente los errores.

2. **Acceder como usuario (GET /user/login)**:
   - Verificación de la funcionalidad de inicio de sesión utilizando las credenciales correctas e incorrectas.
   - Validación de la devolución de un token de sesión válido al iniciar sesión correctamente.

3. **Obtener mascotas por estado (GET /pet/findByStatus)**:
   - Filtrado de mascotas por estado (disponible, pendiente, vendida).
   - Pruebas con estados válidos e inválidos para verificar la respuesta correcta o el manejo de errores.

## Análisis de Resultados
- **Caso Positivo (Crear usuario)**: La API respondió correctamente con un código 200 OK y un mensaje de éxito cuando se crearon los usuarios con todos los campos necesarios.
- **Caso Negativo (Crear usuario sin datos obligatorios)**: La API devolvió un error 400 (Bad Request) cuando se intentó crear un usuario sin el campo obligatorio `lastName`.
- **Acceso de Usuario**: Con credenciales válidas, la API devolvió un token de acceso, y con credenciales incorrectas, devolvió un error 401 (Unauthorized).
- **Obtener mascotas por estado**: Se obtuvieron resultados esperados con estados válidos, y con estados inválidos, la API devolvió un error 400.

## Conclusiones
Este proyecto me permitió comprender mejor cómo funcionan las APIs RESTful y cómo realizar pruebas funcionales en entornos de desarrollo.  
- **Fortalezas**: La API Petstore es una excelente base para entender cómo interactuar con servicios web.  
- **Áreas de mejora**: Las pruebas podrían expandirse para incluir pruebas de seguridad y rendimiento.

Este proyecto no solo validó las funcionalidades de la API, sino que también mejoró mi capacidad para escribir pruebas de integración y garantizar la calidad del software.

## Instrucciones para Ejecutar las Pruebas
1. **Pre-requisitos**:
   - Instalar **Postman** en tu máquina.
   - Clonar o descargar este repositorio.
   - Importar la colección de Postman desde el archivo `Petstore API Tests.postman_collection.json`.

2. **Ejecutar las pruebas**:
   - Abre Postman y carga la colección `Petstore API Tests`.
   - Para cada caso de prueba, realiza la solicitud correspondiente (POST o GET).
   - Verifica las respuestas y asegúrate de que los resultados coincidan con los resultados esperados.

## Contacto
https://www.linkedin.com/in/maurobecerragalvan/
