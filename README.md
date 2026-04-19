# 📚 Aura Library — Sistema Inteligente de Gestión Bibliotecaria

![Status](https://img.shields.io/badge/Status-Desarrollo%20Finalizado-success?style=for-the-badge)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![WPF](https://img.shields.io/badge/WPF-512BD4?style=for-the-badge&logo=.net&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)

Aura Library es una solución tecnológica de vanguardia diseñada originalmente para el Politécnico Santiago Mariño (Extensión Porlamar) como un proyecto estudiantil. El sistema representa un caso de éxito en la modernización de software, tras haber sido migrado desde un entorno legacy basado en Visual Basic y WinForms hacia una arquitectura robusta y escalable en C# con WPF. Esta transición no solo permitió alcanzar una interfaz responsiva y de nivel premium, sino que optimizó el rendimiento operativo mediante un diseño orientado a objetos.

Más allá de la administración convencional, el sistema integra un motor de Inteligencia Artificial que permite la interacción con la base de datos mediante procesamiento de lenguaje natural. Esta capacidad facilita consultas complejas de manera intuitiva, garantizando una trazabilidad absoluta de la información y elevando significativamente la experiencia del usuario final.
---

## 🧠 Aura AI: Asistente Virtual Integrado

El núcleo de innovación de este proyecto es **Aura AI**, un módulo de asistencia inteligente diseñado para:
* **Consultas Dinámicas:** El bibliotecario puede realizar preguntas complejas (ej. *"¿Quién es el lector con más préstamos atrasados?"* o *"¿Cuál es la tendencia de lectura este mes?"*) y recibir respuestas inmediatas analizando la base de datos en tiempo real.
* **Procesamiento de Lenguaje Natural (NLP):** Integración con modelos de IA para convertir datos crudos en información estratégica.
* **Interfaz de Chat Fluida:** Ventana de chat minimalista y asíncrona que no interrumpe el flujo de trabajo principal.

---

## ☁️ Arquitectura de Sincronización Híbrida

Para garantizar la protección del patrimonio informativo, el sistema implementa un modelo de almacenamiento dual:
1.  **Persistencia Local:** Motor SQLite optimizado para operaciones de alta velocidad sin dependencia de internet.
2.  **Respaldo en la Nube (OneDrive):** Sincronización automática de la base de datos con Microsoft OneDrive. Al iniciar sesión, el sistema valida la versión más reciente del archivo, permitiendo la recuperación inmediata ante fallos de hardware o pérdida de datos locales.

---

## ✨ Características Destacadas

* 📊 **Dashboard Analítico:** Panel de control con estadísticas en tiempo real (Libros totales, usuarios activos y "Lectores Estrella").
* 🔄 **Ciclo de Préstamos Inteligente:** * Sistema de alertas visuales por colores para préstamos vencidos o próximos a vencer.
    * Regla de negocio estricta: Máximo 3 préstamos simultáneos por usuario.
* 👥 **Gestión de Usuarios con Blindaje:** Validación triple para evitar duplicados (CI, Correo y Teléfono) antes de la persistencia.
* 🖨️ **Módulo de Reportes Pro:** Generación de documentos detallados en **PDF** (vía QuestPDF) y **Excel** (vía ClosedXML) con filtros temporales y de estado.
* 📦 **UI/UX Moderna:** Interfaz "Borderless" basada en WPF con paginación dinámica de registros y navegación fluida mediante Sidebar asíncrona.
* ⚡ **Arquitectura Asíncrona (Async/Await):** Implementación de tareas en segundo plano para procesos pesados (como subida a la nube o consultas de IA), evitando que la interfaz de usuario se congele.
* 🚀 **Evolución Tecnológica:** Proyecto migrado exitosamente de un entorno legacy (Visual Basic/WinForms) a una arquitectura moderna (C#/WPF), optimizando el rendimiento y la escalabilidad.

---

## 🔐 Seguridad e Integridad (ACID & Triggers)

El sistema ha sido diseñado bajo estándares de ingeniería de software para ser auditable y seguro:
* **Transacciones ACID:** Operaciones críticas (Préstamos/Devoluciones) envueltas en bloques transaccionales. Si una actualización de stock falla, el sistema revierte todos los cambios automáticamente.
* **Auditoría por Triggers:** El historial de movimientos es gestionado directamente por la base de datos mediante disparadores (`Triggers`). Esto garantiza que cada cambio sea inmutable y rastreable, independientemente de la lógica del frontend.
* **Protección SQL:** Implementación estricta de consultas parametrizadas para neutralizar cualquier intento de SQL Injection.

---

## 🛠️ Stack Tecnológico

**Core & Runtime:** C# en .NET 10.0 (LTS) — Seleccionado por su alto rendimiento y compatibilidad extendida.

**Interfaz de Usuario (UI):** WPF (Windows Presentation Foundation) con arquitectura asíncrona para una experiencia fluida.

**Persistencia de Datos:** SQLite bajo una arquitectura de Capa de Acceso a Datos (DAL), garantizando el desacoplamiento y la seguridad de la información.

**Inteligencia Artificial:** Integración de LLM (Large Language Models) para consultas dinámicas en lenguaje natural.

**Ecosistema de Librerías:**

**QuestPDF:** Para la generación de reportes estructurales en PDF.

**ClosedXML:** Para la gestión y exportación de datos a Excel.

**Microsoft.Data.Sqlite:** Para una manipulación eficiente y segura de la base de datos local.

---

## 👤 Autor

**Enzo Rodríguez** — *Estudiante de Ingeniería de Sistemas (PSM Porlamar)*
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/enzo-rodr%C3%ADguez-47756a404/)
 
---
