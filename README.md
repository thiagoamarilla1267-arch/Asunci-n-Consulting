# Asunción Consulting – Security Manager

Prototipo académico para el Tema 5 de TIC: Seguridad de la Información, Cifrado de Datos y Gestión de Respaldos.

## Publicar en GitHub Pages
1. Crear un repositorio público en GitHub, por ejemplo `asuncion-consulting-security`.
2. Subir `index.html` a la raíz del repositorio.
3. Entrar en **Settings → Pages**.
4. En **Build and deployment**, elegir **Deploy from a branch**.
5. Seleccionar la rama `main` y la carpeta `/ (root)`, y guardar.
6. Esperar la publicación. GitHub mostrará el enlace del sitio.

## Funciones
- Panel de control con indicadores y actividad.
- Alta y baja de clientes de demostración.
- Cifrado y descifrado real de archivos en el navegador con Web Crypto API: AES-256-GCM y derivación PBKDF2-SHA-256.
- Exportación y restauración de los registros del prototipo en JSON.
- Registro y resolución de incidentes.
- Simulación didáctica del flujo de backup de Cobian Reflector y Duplicati y de la regla 3-2-1.

## Importante: alcance académico
- La aplicación no instala ni ejecuta Cobian Reflector o Duplicati. Representa su flujo de trabajo para la demostración del tema.
- El backup JSON exporta los registros de esta aplicación, no los archivos originales de la computadora.
- Los datos de clientes se guardan en el almacenamiento local del navegador (`localStorage`); no hay servidor, usuarios ni sincronización entre equipos.
- El cifrado de archivos sí se ejecuta en el navegador. La contraseña no se transmite. Si se pierde, el archivo no se puede recuperar.
- Para archivos reales de clientes, usar un entorno aprobado por la organización y políticas de seguridad adecuadas. No subir datos personales ni contables al repositorio de GitHub.
- Para que Web Crypto funcione, publicar el sitio mediante HTTPS (GitHub Pages lo proporciona).
