4. Software Necesario
Para el desarrollo en la asignatura de Lenguaje de Marcas y Entornos de Desarrollo, utilizaremos dos herramientas fundamentales: un editor de código ligero y versátil (Visual Studio Code) y un entorno de desarrollo integrado (IDE) completo para proyectos más complejos (Apache NetBeans). A continuación, se detalla el listado, los enlaces de descarga y las guías básicas de instalación para ambos.

4.1. Visual Studio Code (VS Code)
Visual Studio Code es un editor de código fuente ligero pero potente, disponible para Windows, macOS y Linux. Incluye soporte integrado para JavaScript, TypeScript y Node.js, y cuenta con un rico ecosistema de extensiones para otros lenguajes como Python, Java, PHP, C++, C# y, por supuesto, HTML, CSS y XML .

Listado de características principales:
Multiplataforma: Compatible con Windows, macOS y Linux .

Gratuito y de código abierto .

IntelliSense: Autocompletado inteligente de código más potente que el autocompletado tradicional .

Depurador integrado: Permite depurar código directamente desde el editor .

Control de versiones integrado (Git): Soporte nativo para Git, con interfaz gráfica para commits, pulls y pushes .

Terminal integrada: Permite ejecutar comandos sin salir del editor.

Extensiones: Gran cantidad de extensiones para personalizar y añadir funcionalidades .

Enlace de descarga:
Página oficial: https://code.visualstudio.com/ 

Guía básica de instalación:
La página de descarga de VS Code detecta automáticamente tu sistema operativo y sugiere la versión adecuada .

Instalación en Windows:

Una vez en la página oficial, haz clic en el botón "Download for Windows" .

Ejecuta el archivo descargado (por ejemplo, VSCodeUserSetup-x64-1.81.0.exe) .

Acepta el contrato de licencia.

Selecciona la carpeta de instalación (por defecto suele ser en C:\Program Files\Microsoft VS Code) .

En la pantalla "Seleccionar tareas adicionales", es recomendable marcar las siguientes opciones para una mejor experiencia:

"Agregar acción 'Abrir con Code' al menú contextual de archivos de Windows Explorer".

"Agregar acción 'Abrir con Code' al menú contextual de directorios de Windows Explorer".

"Registrar Code como editor para tipos de archivo compatibles".

"Agregar a la variable de entorno PATH" (esto permite abrir VS Code desde la línea de comandos con code .) .

Haz clic en "Instalar" y, al finalizar, en "Finalizar". Puedes mantener marcada la casilla "Iniciar Visual Studio Code" para abrirlo inmediatamente .

Instalación en macOS:

En la página oficial, haz clic en el botón "Download for macOS".

Abre el archivo .zip descargado. Esto extraerá la aplicación Visual Studio Code.app.

Arrastra la aplicación Visual Studio Code.app a la carpeta "Applications". Esto hará que esté disponible en el Launchpad .

Para ejecutarlo, ve a la carpeta "Applications" y haz doble clic en "Visual Studio Code".

Instalación en Linux (ejemplo para distribuciones basadas en Debian/Ubuntu):

En la página oficial, haz clic en el botón "Download for Linux" (generalmente ofrece paquetes .deb y .rpm).

Descarga el archivo .deb.

Abre una terminal y navega hasta la carpeta donde se descargó el archivo (normalmente ~/Descargas o ~/Downloads).

Instala el paquete con el siguiente comando (reemplaza nombre-del-archivo.deb por el nombre real del archivo descargado) :

bash
sudo dpkg -i nombre-del-archivo.deb
Si hay dependencias faltantes, ejecuta:

bash
sudo apt install -f
Configuración inicial post-instalación:

Idioma: Para usar VS Code en español, abre la aplicación, ve a la vista de extensiones (Ctrl+Shift+X), busca "Spanish Language Pack" y haz clic en Instalar. Luego reinicia el editor .

Tema: Puedes cambiar el tema de color desde el menú Archivo > Preferencias > Tema de color .

4.2. Apache NetBeans
Apache NetBeans es un entorno de desarrollo integrado (IDE) de código abierto, escrito en Java, que permite desarrollar aplicaciones de escritorio, móviles y web con Java, así como soporte para otros lenguajes como HTML5, PHP, C/C++ y más . Es un proyecto de la Apache Software Foundation.

Listado de características principales:
Potente IDE para Java: Soporte completo para desarrollo en Java SE, Java EE y Java ME .

Multi-lenguaje: Soporte para PHP, HTML5, JavaScript, Groovy, C y C++ .

Gestión de proyectos: Organización eficiente de proyectos y dependencias.

Refactorización y herramientas de código: Herramientas avanzadas para mejorar y mantener la calidad del código.

Integración con control de versiones: Soporte integrado para Git, Subversion y Mercurial .

Nota importante: A partir de Apache NetBeans 26, el proyecto oficial ya no proporciona instaladores directamente (archivos .exe para Windows o .dmg para macOS) . En su lugar, se ofrecen paquetes ZIP independientes de la plataforma (para Windows, Linux) y enlaces a instaladores mantenidos por la comunidad.

Enlace de descarga:
Página oficial de descargas de Apache NetBeans: https://netbeans.apache.org/download/index.html 

En esta página encontrarás:

Platform-Independent Zip: Archivo ZIP que funciona en cualquier sistema con Java instalado. Es la opción más universal y recomendada.

Installers: Enlaces a instaladores mantenidos por la comunidad para facilitar la instalación en diferentes sistemas operativos .

Guía básica de instalación:
Requisito previo: Apache NetBeans requiere que Java Development Kit (JDK) esté instalado en tu sistema para funcionar correctamente. Asegúrate de tener JDK 17 o superior .

Instalación en Windows, macOS y Linux (usando el ZIP independiente):

Esta es la forma más directa y funciona en todos los sistemas operativos.

Descargar el ZIP: En la página de descargas de Apache NetBeans, selecciona la última versión (por ejemplo, "Apache NetBeans 27") y descarga el archivo "Platform-Independent Zip" (por ejemplo, apache-netbeans-27-bin.zip).

Extraer el ZIP: Extrae el contenido del archivo ZIP en la carpeta donde desees instalar NetBeans. Ejemplos de rutas recomendadas:

Windows: C:\Program Files\NetBeans o C:\Users\TuUsuario\NetBeans.

macOS/Linux: /home/tu-usuario/netbeans o /opt/netbeans.

Ejecutar NetBeans: Dentro de la carpeta extraída, busca y ejecuta el archivo:

Windows: bin/netbeans64.exe (o netbeans.exe).

macOS/Linux: bin/netbeans.

(Opcional) Crear un acceso directo: Puedes crear un acceso directo a este ejecutable en tu escritorio o menú de aplicaciones.

Instalación en Debian/Ubuntu (usando paquete .deb):
Si prefieres una instalación más integrada en el sistema, puedes optar por el paquete .deb .

Descargar el .deb: En la página de descargas, busca el enlace a "Community provided installers" o ve directamente a la sección de descargas de la versión específica (ej. para la versión 25) y descarga el archivo apache-netbeans_25-1_all.deb .

Abrir una terminal en la carpeta donde se descargó el archivo.

Ejecutar los comandos de instalación :

bash
sudo apt install wget
wget https://www.apache.org/dyn/closer.lua/netbeans/netbeans-installers/25/apache-netbeans_25-1_all.deb
sudo apt install ./apache-netbeans_25-1_all.deb
(Nota: La URL de wget puede variar según la versión; es mejor obtener el enlace directo desde la página de descargas).

Instalación en Arch Linux:
NetBeans está disponible en los repositorios oficiales .

bash
sudo pacman -S netbeans
