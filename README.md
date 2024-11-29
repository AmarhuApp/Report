# Proyecto Amarhu

### Informe de Conversión de Python a Java

---

## Descripción

Conversión y desarrollo de la aplicación web Amarhu para **Prensa Alternativa El Jota**, destinada a la visualización y análisis de rendimiento audiovisual.

---

## Integrantes del Proyecto

- **Jose Del Castillo** / Director General
- **George Galván** / Desarrollador Principal
- **Sebastian Ramirez** / Desarrollador Principal

---

## Contenido

1. [Introducción](#introducción)
2. [Antecedentes](#antecedentes)
    - [Estado Actual del Proyecto en Python](#estado-actual-del-proyecto-en-python)
    - [Problemas Identificados en la Versión Original](#problemas-identificados-en-la-versión-original)
    - [Justificación para la Migración a Java](#justificación-para-la-migración-a-java)
3. [Entrevistas y Requisitos](#entrevistas-y-requisitos)
    - [Objetivo de las Entrevistas con Usuarios](#objetivo-de-las-entrevistas-con-usuarios)
    - [Análisis de Requisitos Recolectados](#análisis-de-requisitos-recolectados)
    - [Cambios Clave a Realizar según las Entrevistas](#cambios-clave-a-realizar-según-las-entrevistas)
    - [Imágenes y Enlaces a las Entrevistas](#imágenes-y-enlaces-a-las-entrevistas)
4. [Arquitectura del Proyecto en Java](#arquitectura-del-proyecto-en-java)
5. [Tecnologías Utilizadas](#tecnologías-utilizadas)
6. [Diseño y Planificación de la Interfaz de Usuario](#diseño-y-planificación-de-la-interfaz-de-usuario)
7. [Implementación Técnica](#implementación-técnica)
8. [Manejo de Consultas y Visualización de Informes](#manejo-de-consultas-y-visualización-de-informes)
9. [Evaluación de Resultados](#evaluación-de-resultados)
10. [Conclusión](#conclusión)
11. [Anexos](#anexos)
12. [Product Backlog](#product-backlog)

---

## 1. Introducción

El proyecto **Amarhu** surge como una solución web dirigida a los trabajadores de **Prensa Alternativa El Jota**, diseñada específicamente para optimizar el acceso y análisis del rendimiento de su producción audiovisual. La aplicación implementará un sistema de roles y herramientas de análisis avanzado que incluyen gráficos interactivos, estadísticas en tiempo real y filtros personalizados.

---

## 2. Antecedentes

### 2.1 Estado Actual del Proyecto en Python

La versión actual utiliza hojas de cálculo en Excel como principal medio para almacenar y presentar información. Este enfoque presenta limitaciones considerables en términos de usabilidad, acceso y análisis.

### 2.2 Problemas Identificados en la Versión Original

- Manejo excesivo de múltiples hojas de cálculo individuales.
- Dificultad para realizar análisis comparativos en tiempo real.
- Limitaciones en la incorporación de herramientas visuales avanzadas.

### 2.3 Justificación para la Migración a Java

Migrar a una plataforma web basada en Java permitirá aprovechar herramientas como gráficos interactivos y filtros dinámicos, facilitando la interpretación de datos de manera eficiente.

---

## 3. Entrevistas y Requisitos

### 3.1 Objetivo de las Entrevistas con Usuarios

Identificar problemas en la versión actual y recopilar expectativas para la nueva aplicación web.

### 3.2 Análisis de Requisitos Recolectados

- Filtros dinámicos.
- Organización de botones y elementos de la interfaz.
- Representación visual con gráficos interactivos.

### 3.3 Cambios Clave a Realizar según las Entrevistas

- Inclusión de filtros avanzados.
- Diseño de interfaz optimizado.
- Incorporación de gráficos interactivos.

---

## 4. Arquitectura del Proyecto en Java

### 4.1 Estructura Modular Basada en Bounded Contexts

El proyecto sigue los principios de **MVC** y **DDD**, organizando el sistema en módulos desacoplados para facilitar su escalabilidad.

### 4.2 Estructura de Bounded Contexts

- **YouTube**: Gestión de datos y estadísticas.
- **Empleados**: Gestión de roles y usuarios.
- **Reportes**: Generación y manejo de informes.

### 4.3 Principales Componentes dentro de cada Bounded Context

- **Controladores**: Manejo de solicitudes HTTP.
- **Servicios**: Lógica de negocio.
- **DTOs y Mappers**: Transferencia de datos al frontend.
- **Excepciones**: Manejo de errores.

---

## 5. Tecnologías Utilizadas

### 5.1 Backend: Java y Spring Boot

- Java para lógica robusta.
- Spring Boot para integración rápida con herramientas de seguridad, persistencia y APIs.

### 5.2 Frontend: Vue.js

- Simplicidad y modularidad para construir interfaces reactivas.
- Comunicación eficiente con el backend mediante Axios.

---

## 6. Diseño y Planificación de la Interfaz de Usuario

El diseño incluirá gráficos dinámicos y filtros avanzados para facilitar el análisis interactivo.

---

## 7. Implementación Técnica

### 7.1 Configuración del Proyecto en Java

Estructura modular con bounded contexts para YouTube, Empleados y Reportes.

### 7.2 Migración de Funciones de Python a Java

Transformación de lógica de negocio en servicios de backend con JPA y consultas optimizadas.

---

## 8. Manejo de Consultas y Visualización de Informes

### 8.1 Estructura de Consultas

Consultas segmentadas por roles, incluyendo filtros avanzados y estadísticas agregadas.

---

## 9. Evaluación de Resultados

- Comparación del desempeño entre las versiones en Python y Java.
- Cumplimiento de requisitos y retroalimentación de usuarios.

---

## 10. Conclusión

### 10.1 Logros del Proyecto

- Migración exitosa.
- Implementación de herramientas avanzadas de análisis.

### 10.2 Recomendaciones para el Futuro

- Ampliar las funcionalidades basadas en el feedback de usuarios.

---

## 11. Anexos

- Entrevistas y Encuestas.
- Diagramas Adicionales.
- Código de Ejemplo.

---

## 12. Product Backlog

El Product Backlog incluye todas las funcionalidades esenciales priorizadas para garantizar un MVP funcional en **60 story points**. La integración cubre todas las opciones del sidebar, perfil de usuario y jerarquías.

---

### **1. Frontend (Vue.js)**

| **ID**   | **Descripción**                                                      | **Story Points** | **Prioridad** |
|----------|----------------------------------------------------------------------|-------------------|---------------|
| FE-001   | Configurar entorno inicial (Vue, Vite, dependencias).                | 2                 | Alta          |
| FE-002   | Crear estructura básica de componentes (Header, Sidebar, NewsFeed).  | 3                 | Alta          |
| FE-003   | Implementar vista Home con estadísticas generales y rendimiento del último video. | 5       | Alta          |
| FE-004   | Crear vista Posts para gestionar noticias y publicaciones.           | 3                 | Alta          |
| FE-005   | Implementar perfil de usuario con opciones para ver jerarquías y permisos. | 5        | Alta          |
| FE-008   | Adaptar diseño responsive para diferentes dispositivos.              | 5                 | Alta          |

**Subtotal Frontend**: **23 story points.**

---

### **2. Backend (Spring Boot)**

| **ID**   | **Descripción**                                                       | **Story Points** | **Prioridad** |
|----------|-----------------------------------------------------------------------|-------------------|---------------|
| BE-001   | Configurar entorno inicial (Spring Boot, MySQL/PostgreSQL, dependencias). | 3             | Alta          |
| BE-002   | Implementar sistema de autenticación y autorización con jerarquías de usuarios (JWT). | 8         | Alta          |
| BE-003   | Crear entidades principales: `User`, `Video`, `Post`.                 | 5                 | Alta          |
| BE-004   | Implementar servicios para consumir YouTube Data API (metadatos de videos). | 8            | Alta          |
| BE-006   | Crear endpoints REST para manejar videos y estadísticas.              | 5                 | Alta          |
| BE-007   | Crear endpoints REST para CRUD de noticias y publicaciones.           | 5                 | Alta          |

**Subtotal Backend**: **34 story points.**

---

### **3. Integración**

| **ID**   | **Descripción**                                                         | **Story Points** | **Prioridad** |
|----------|-------------------------------------------------------------------------|-------------------|---------------|
| INT-001  | Conectar frontend con backend para Home (último video y estadísticas generales). | 5           | Alta          |
| INT-002  | Conectar frontend con backend para Posts (gestión de noticias).         | 5                 | Alta          |
| INT-003  | Conectar frontend con backend para Perfil de usuario (jerarquías, permisos). | 5         | Alta          |

**Subtotal Integración**: **15 story points.**

---

### **4. Metas Finales**

| **ID**   | **Descripción**                                        | **Story Points** | **Prioridad** |
|----------|--------------------------------------------------------|-------------------|---------------|
| MF-001   | Despliegue en un entorno productivo (Frontend y Backend). | 5             | Alta          |
| MF-003   | Documentación del proyecto (manuales, guías técnicas). | 1                 | Media         |

**Subtotal Metas Finales**: **6 story points.**

---

### **Resumen por Áreas**

| **Área**       | **Story Points** |
|----------------|-------------------|
| Frontend       | 23                |
| Backend        | 34                |
| Integración    | 15                |
| Metas Finales  | 6                 |
| **Total**      | **60**            |

---

### **Plan de Trabajo (60 Story Points en 60 Días Laborales)**

#### **Semana 1-2**:
- Configuración de entornos iniciales (FE-001, BE-001).
- Creación de entidades principales (BE-003).
- Implementación de estructura básica de componentes (FE-002).

#### **Semana 3-4**:
- Desarrollo de vista Home y Posts (FE-003, FE-004).
- Implementación de servicios y endpoints para estadísticas, noticias y jerarquías (BE-004, BE-006, BE-007, BE-002).

#### **Semana 5-6**:
- Implementación del perfil de usuario con jerarquías y permisos (FE-005).
- Conexión frontend-backend para Home, Posts y Perfil de usuario (INT-001, INT-002, INT-003).
- Adaptación del diseño responsive (FE-008).

#### **Semana 7-8**:
- Pruebas de integración y ajustes finales.
- Despliegue del proyecto y documentación básica (MF-001, MF-003).

🎯 **Resultado Final**: Un MVP funcional en **60 story points**, cubriendo las funcionalidades críticas para un despliegue exitoso.



