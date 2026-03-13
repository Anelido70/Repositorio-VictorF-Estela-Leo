# Apuntes Extendidos: Prácticas de Software, Git, GitHub y Personalización de IDEs

## 1. Prácticas de Software y Control de Versiones

### 1.1. ¿Qué es el Control de Versiones?
El control de versiones, también conocido como VCS (Version Control System), es una clase de herramientas esenciales en cualquier flujo de trabajo de desarrollo moderno [citation:2]. Un sistema de control de versiones permite a un grupo de desarrolladores trabajar en la misma base de código sin interferir entre sí, y facilita volver a estados anteriores del código si es necesario [citation:2].

### 1.2. Git: El Sistema de Control de Versiones Distribuido
Git es un sistema de control de versiones distribuido creado por Linus Torvalds en 2005 para gestionar el desarrollo del kernel de Linux [citation:6]. Sus características principales incluyen:
- **Repositorios distribuidos y seguros**: Cada desarrollador tiene una copia completa del historial del proyecto, lo que permite trabajar de forma offline y ofrece robustez [citation:9].
- **Integridad**: Utiliza un algoritmo de hash seguro (SHA-1) para generar identificadores únicos de 40 dígitos para cada commit, funcionando como una firma que garantiza la confiabilidad del versionado [citation:9].
- **Eficiencia**: Gestiona ramas y merges de manera muy ligera y rápida.

### 1.3. Buenas Prácticas Esenciales con Git
Adoptar buenas prácticas desde el principio es crucial para mantener un historial de proyecto limpio y facilitar la colaboración.

- **Commits Atómicos y Frecuentes**: Realiza commits pequeños y enfocados en un solo cambio o funcionalidad. Esto facilita la revisión, la depuración y la reversión de cambios si algo sale mal [citation:4]. Un commit debe representar un punto lógico en el historial que estás guardando [citation:3][citation:10].
- **Mensajes de Commit Descriptivos**: Un buen mensaje de commit explica el "qué" y el "por qué" del cambio, no el "cómo" [citation:3][citation:10].
    - **Asunto (Línea 1)**: Usa el imperativo en tiempo presente. Debe completar la frase: "Si se aplica, este commit hará..." [citation:3][citation:10]. Ejemplo: "Añade función de validación de email" en lugar de "Añadida función" o "Cambios".
    - **Cuerpo (Opcional)**: Explica la motivación del cambio y contrasta con el comportamiento anterior [citation:3][citation:5][citation:10].
- **Trabajar con Ramas (Branches)**: Nunca trabajes directamente en la rama principal (`main` o `master`). Crea una nueva rama para cada característica, corrección de error o tarea [citation:1][citation:4]. Esto protege la integridad del código base principal y permite un flujo de desarrollo más organizado [citation:1]. Usa nombres descriptivos para las ramas, como `feature/autenticacion-google` o `fix/error-en-formulario` [citation:1].
- **Ignorar Archivos Innecesarios**: Utiliza un archivo `.gitignore` para evitar que archivos temporales, de configuración local, dependencias o secretos (como claves SSH o contraseñas) se suban al repositorio [citation:3][citation:6][citation:10]. Puedes encontrar plantillas útiles en [github/gitignore](https://github.com/github/gitignore) [citation:3][citation:10].
- **Sincronización Constante**: Antes de empezar a trabajar y antes de subir cambios, sincroniza tu repositorio local con el remoto usando `git pull` para evitar conflictos [citation:4].

## 2. GitHub: La Plataforma para Alojar y Colaborar

### 2.1. ¿Qué es GitHub?
GitHub es una aplicación web que proporciona herramientas útiles basadas en Git para alojar repositorios de código en la nube y facilitar la colaboración [citation:2][citation:9]. Actúa como un "remote repository" (repositorio remoto) que guarda los versionamientos de tu código Git, permitiendo el trabajo en equipo y la contribución a proyectos de código abierto [citation:9].

### 2.2. Configuración Inicial para Trabajar con GitHub
Antes de interactuar con GitHub, necesitas realizar una configuración básica.

- **Instalar Git**: Descarga e instala Git desde [git-scm.com](https://git-scm.com/) [citation:2][citation:3][citation:4].
- **Crear una Cuenta en GitHub**: Regístrate en [GitHub.com](https://github.com/) [citation:2][citation:3][citation:7].
- **Configurar Git Localmente**: Establece tu identidad, ya que cada commit la usará [citation:3][citation:10].
    ```bash
    git config --global user.name "Tu Nombre"
    git config --global user.email "tu-email@example.com"
    git config --list # Para verificar la configuración
