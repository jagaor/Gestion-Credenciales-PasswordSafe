# Gestión Segura de Credenciales con Password Safe

## 📝 Descripción General
Este proyecto forma parte del módulo de "Bastionado de Redes y Sistemas" y aborda uno de los pilares fundamentales de la ciberseguridad: la gestión robusta de identidades y contraseñas. La práctica documenta la implementación y el uso de **Password Safe**, un gestor de contraseñas de código abierto diseñado por Bruce Schneier, evaluando su despliegue y operatividad tanto en sistemas operativos Windows como en distribuciones Linux.

## 🎯 Objetivos del Proyecto
* Concienciar sobre los riesgos de la reutilización de contraseñas y el almacenamiento en texto plano.
* Instalar y configurar Password Safe en entornos multiplataforma (Windows y Linux).
* Crear y asegurar bases de datos de contraseñas (archivos `.psafe3`) mediante algoritmos de cifrado fuerte.
* Establecer políticas de acceso seguras mediante el uso de una "Master Password" (Contraseña Maestra) robusta.
* Administrar el ciclo de vida de las credenciales: añadir nuevas entradas, clasificar por grupos y utilizar el generador automático de contraseñas seguras.

## 🛠️ Tecnologías y Herramientas
* **Software de Gestión**: Password Safe.
* **Sistemas Operativos**: Windows 10/11 y Linux (entorno Kali/Debian).
* **Criptografía**: Cifrado Twofish (estándar de Password Safe) para la protección de la base de datos local.

## ⚙️ Detalles de Implementación Destacados
* **Despliegue Multiplataforma**: Se documentó el proceso completo de instalación, contrastando las diferencias entre el entorno gráfico nativo de Windows y la instalación mediante repositorios/paquetes en Linux.
* **Creación de la Bóveda Segura**: Se generó un archivo de base de datos encriptado y se protegió con una contraseña maestra de alta entropía, garantizando que el acceso a las credenciales almacenadas sea inviable en caso de exfiltración del archivo físico.
* **Organización y Categorización**: Se demostró el uso operativo de la herramienta creando grupos de credenciales (por ejemplo, accesos a máquinas "Kali", credenciales de administración, etc.), almacenando para cada entrada el usuario, la contraseña, la URL asociada y notas adicionales.
* **Uso del Portapapeles Seguro**: Se evaluó la capacidad de la herramienta para copiar credenciales temporalmente al portapapeles y borrar su rastro rápidamente, mitigando el riesgo de robo por software malicioso (clipboard loggers).

## 📄 Documentación Completa
Para revisar el proceso de instalación paso a paso con capturas de pantalla, la configuración de la contraseña maestra y la creación de entradas en la bóveda, puedes consultar la memoria técnica del proyecto:

👉 [Enlace al Informe Técnico en Google Drive](https://docs.google.com/document/d/1TNupllI-sRYfNfZIgpVa2uiUVoHfaLc4ZN-afv319tA/edit?usp=sharing)

## ⚠️ Aviso Legal / Ética
*Este documento ha sido elaborado con fines formativos para la asignatura de Bastionado de Redes y Sistemas, fomentando las buenas prácticas en la gestión de contraseñas personales y corporativas.*
