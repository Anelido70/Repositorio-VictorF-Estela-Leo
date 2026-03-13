# Apuntes Extendidos de XML: Guía Completa

## 1. Introducción a XML

### 1.1. ¿Qué es XML?
XML (eXtensible Markup Language), o Lenguaje de Marcado Extensible, es un lenguaje de marcado desarrollado por el W3C (World Wide Web Consortium) que define un conjunto de reglas para codificar documentos de forma que sean legibles tanto por humanos como por máquinas .

A diferencia de HTML, que está diseñado para mostrar datos y tiene un conjunto predefinido de etiquetas, XML está diseñado para **transportar y almacenar datos**, y permite a los usuarios **definir sus propias etiquetas** personalizadas .

### 1.2. Características Principales de XML
- **Extensible**: Los usuarios pueden crear sus propias etiquetas y atributos según sus necesidades .
- **Estructurado**: Organiza la información de forma jerárquica y árbol, facilitando su comprensión y procesamiento .
- **Autodescriptivo**: La estructura y las etiquetas suelen describir el significado de los datos que contienen .
- **Neutral/Independiente**: Es independiente de la plataforma, el software y el hardware, lo que lo hace ideal para el intercambio de datos entre sistemas dispares .
- **Basado en texto**: Al ser texto plano, es legible y fácil de depurar.

### 1.3. ¿Para qué se usa XML?
- **Intercambio de datos entre sistemas**: Es un formato estándar para que aplicaciones escritas en diferentes lenguajes o que corren en diferentes plataformas puedan comunicarse .
- **Almacenamiento de configuración**: Muchas aplicaciones (como servidores o IDEs) usan archivos XML para guardar su configuración.
- **Formatos de documentos ofimáticos**: Formatos como .docx (Word), .xlsx (Excel) y .odt (LibreOffice) son, en esencia, archivos ZIP que contienen múltiples archivos XML.
- **Sindicación de contenido (RSS/Atom)**: Los feeds de noticias y blogs utilizan XML para distribuir contenido actualizado .
- **Servicios Web (SOAP, XML-RPC)**: Protocolos de comunicación entre sistemas basados en XML.

## 2. Estructura Básica de un Documento XML

Un documento XML bien formado debe seguir una estructura específica.

### 2.1. Prólogo (Declaración XML)
Es la primera línea de un documento XML y define la versión de XML y la codificación de caracteres utilizada.
```xml
<?xml version="1.0" encoding="UTF-8"?>
