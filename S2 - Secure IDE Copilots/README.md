# AI Workshop - S2 IDE Copilots & Advanced Prompting 🧠

Este módulo documenta el uso profesional de copilotos de IDE (GitHub Copilot/Cursor) y la implementación de un **Framework de Prompting Estructurado** para el desarrollo de software robusto.

## 🚀 Objetivos de la Sesión
El trabajo se ha centrado en la creación y optimización de un sistema de captura de datos seguro, aplicando tres niveles de interacción con la IA:

1.  **Módulo de Contacto (`/contact`)**:
    - Implementación de un formulario con **Validación Dual** (Cliente/Servidor).
    - Lógica de saneamiento contra ataques **XSS** y **Inyección**.
2.  **Pipeline de Refactorización**:
    - Reestructuración de código existente mediante prompts de arquitectura.
    - Aplicación del **Principio de Responsabilidad Única (SRP)** para desacoplar validaciones de la lógica de negocio.

## 🛠️ Framework de Prompting (The 5 Pillars)
Para garantizar resultados de "Nivel Senior" y evitar la ambigüedad, cada componente fue generado siguiendo este protocolo:
* **ROLE**: Definición de seniority (Senior Fullstack / Security Expert).
* **CONTEXT**: Detalles del ecosistema (`AI-Engineering-Workshop`) y stack técnico.
* **INSTRUCTIONS**: Acciones atómicas y claras.
* **CONSTRAINTS**: Límites estrictos (No librerías nuevas, no cambiar firmas de funciones, límites de líneas).
* **ACCEPTANCE**: Criterios de éxito binarios y basados en tests.

## 🛡️ Estándares de Ingeniería Aplicados
- **Signature Preservation**: Refactorización transparente que garantiza la compatibilidad con el frontend existente.
- **Defensive Validation**: Whitelisting de parámetros y control de tipos estricto.
- **Clean Architecture**: Separación de responsabilidades en `Middlewares`, `Handlers` y `Helpers`.

## 📑 Nuevos Endpoints (API Spec)
| Método | Endpoint | Descripción | Validación Clave |
| :--- | :--- | :--- | :--- |
| `POST` | `/contact` | Captura de leads segura | Email RFC 5322 + Max 1000 chars |
| `GET` | `/health` | Estado del sistema | Uso de Memoria < 90% |

## 🤖 Uso de IA en esta Sesión
- **Herramientas**: GitHub Copilot / Cursor para asistencia "Inline".
- **Estrategia**: *Pause-Before-Tab*. Auditoría manual de cada sugerencia para evitar la "Aceptación Pasiva".
- **Refactor**: Uso de IA para identificar deuda técnica y proponer abstracciones basadas en patrones de diseño (Middleware Pattern).

---
*Sesión 2 — IES Rafael Alberti — Javier 2026*
