# Planificación de Proyecto de Software - Sistema de Gestión de Inventario Inteligente (SGII)

## 1. Objetivos

### 1.1 Objetivos Generales

Diseñar e implementar un Sistema de Gestión de Inventario Inteligente (SGII) para una cadena de tiendas minoristas, permitiendo administrar productos, ventas y movimientos de inventario en tiempo real, reduciendo errores operacionales, mejorando la trazabilidad y optimizando la gestión del stock.

### 1.2 Objetivos Específicos

- Digitalizar el control de inventario actualmente realizado de forma manual.
- Centralizar la gestión de productos y movimientos de stock.
- Implementar mecanismos de autenticación y autorización basados en roles.
- Garantizar trazabilidad y auditoría de movimientos de inventario.
- Permitir gestión eficiente de ventas y entradas de productos.
- Implementar alertas automáticas de stock crítico.
- Mejorar la experiencia de usuarios operativos y administrativos.
- Asegurar integridad y consistencia de datos en tiempo real.

---

# 2. Alcance del Proyecto

El Sistema de Gestión de Inventario Inteligente (SGII) tiene como propósito modernizar el control operativo de inventario y ventas dentro de una tienda minorista, reemplazando procesos manuales por una plataforma web centralizada y automatizada.

El sistema permitirá administrar productos, controlar stock en tiempo real, registrar ventas y mantener trazabilidad completa de los movimientos realizados por los usuarios. Además, incorporará mecanismos de seguridad y control de acceso para garantizar integridad y protección de la información.

Dentro del alcance del proyecto se considera:

- Gestión de productos y categorías.
- Control de inventario en tiempo real.
- Registro de entradas y salidas de productos.
- Administración de ventas.
- Gestión de usuarios y roles.
- Generación de alertas de stock crítico.
- Registro de auditoría y trazabilidad.
- Generación de reportes operacionales.
- Plataforma web accesible mediante navegador.

El proyecto no contempla funcionalidades avanzadas externas al objetivo principal del sistema, tales como:

- Aplicación móvil nativa.
- Integración con sistemas ERP empresariales.
- Integración bancaria o pagos en línea.
- Predicción inteligente mediante inteligencia artificial.
- Soporte multiempresa.
- Integraciones con marketplaces externos.

A nivel técnico, el sistema será construido utilizando una arquitectura en capas, permitiendo separar responsabilidades entre interfaz, lógica de negocio y persistencia de datos, facilitando así la mantenibilidad y escalabilidad futura del software.

---

## 2.1 Requerimientos Funcionales

### Gestión de Inventario
- Registrar entrada de productos.
- Actualizar stock.
- Consultar disponibilidad.
- Gestionar movimientos de inventario.
- Generar alertas automáticas.

### Gestión de Ventas
- Registrar ventas.
- Descontar stock automáticamente.
- Consultar historial de ventas.

### Gestión de Usuarios
- Registrar usuarios.
- Gestionar roles y permisos.
- Controlar accesos.

---

## 2.2 Requerimientos No Funcionales

### Seguridad
- Autenticación y autorización.
- Restricción de acceso según roles.
- Auditoría de accesos y modificaciones.

### Disponibilidad
- Disponibilidad superior al 99,5% en horario laboral.

### Rendimiento
- Tiempo de respuesta menor a 100 ms.

---
## 2.3 Priorización MoSCoW

### Must Have
- Registro de ventas.
- Gestión de inventario.
- Gestión de productos.
- Gestión de usuarios y roles.
- Alertas automáticas de stock.
- Auditoría de movimientos.

### Should Have
- Dashboard administrativo.
- Reportes operacionales.
- Historial avanzado de movimientos.

### Could Have
- Integración con lectores de código de barras.
- Notificaciones por correo.
- Panel estadístico avanzado.

### Won’t Have
- Aplicación móvil nativa.
- Inteligencia artificial predictiva.
- Integración ERP avanzada.
- Soporte multiempresa.

---

## 2.4 Diseño de Arquitectura de Alto Nivel

Para el Sistema de Gestión de Inventario Inteligente (SGII) se propone una arquitectura en capas, permitiendo separar responsabilidades y mejorar la mantenibilidad del sistema.

### Capa de Presentación
Encargada de la interfaz web utilizada por vendedores, administradores de bodega y administradores del sistema.

### Capa de Aplicación
Gestiona las solicitudes del usuario mediante controladores y APIs REST, coordinando las operaciones del sistema.

### Capa de Negocio
Contiene las reglas principales del sistema, como validaciones de stock, gestión de ventas, control de permisos y generación de alertas.

### Capa de Datos
Responsable del acceso y persistencia de la información en la base de datos.

### Beneficios de la Arquitectura
- Separación de responsabilidades.
- Mejor escalabilidad.
- Mayor mantenibilidad.
- Facilidad para futuras integraciones.
- Mejor control de seguridad.
---

# 3. Identificación de Stakeholders

| Stakeholder | Influencia | Interés | Estrategia |
|---|---|---|---|
| Gerencia | Alta | Alta | Seguimiento ejecutivo |
| Administrador Sistema | Alta | Alta | Validación continua |
| Administrador Bodega | Media | Alta | Feedback operativo |
| Vendedores | Media | Alta | Validación funcional |

---

# 4. WBS y Cronograma Simplificado

# 4. WBS y Cronograma Simplificado

**Explicación:** PMI define el WBS (Work Breakdown Structure) como una descomposición jerárquica orientada a entregables del trabajo que debe ejecutar el equipo del proyecto. Esta herramienta permite delimitar el alcance, organizar el trabajo y comunicar claramente los entregables del proyecto a todas las partes interesadas.

El WBS del Sistema de Gestión de Inventario Inteligente (SGII) se estructura considerando todos los entregables principales necesarios para el desarrollo, validación e implementación de la plataforma.

---

## 4.1 WBS Simplificado Orientado a Entregables

### 1. Gestión del Proyecto

#### 1.1 Documentación Inicial
- Acta de constitución
- Definición de alcance
- Identificación de stakeholders

#### 1.2 Planificación
- Planificación cronograma
- Planificación recursos
- Planificación riesgos

#### 1.3 Seguimiento y Control
- Reuniones seguimiento
- Control avances
- Gestión cambios

---

### 2. Análisis y Diseño

#### 2.1 Levantamiento de Requerimientos
- Requerimientos funcionales
- Requerimientos no funcionales
- Casos de uso

#### 2.2 Diseño Arquitectura
- Arquitectura en capas
- Diseño componentes
- Diseño seguridad

#### 2.3 Diseño Base de Datos
- Modelo relacional
- Entidades principales
- Relaciones sistema

#### 2.4 Diseño Interfaces
- Wireframes
- Formularios
- Dashboard

---

### 3. Plataforma SGII

#### 3.1 Gestión de Inventario
- Control stock
- Registro movimientos
- Actualización inventario

#### 3.2 Gestión de Productos
- Registro productos
- Edición productos
- Consulta productos

#### 3.3 Gestión de Ventas
- Registro ventas
- Historial ventas
- Actualización stock automática

#### 3.4 Gestión de Usuarios
- Registro usuarios
- Gestión roles
- Control acceso

#### 3.5 Auditoría y Seguridad
- Registro actividades
- Validación permisos
- Trazabilidad movimientos

#### 3.6 Reportes y Alertas
- Alertas stock crítico
- Reportes operacionales
- Dashboard administrativo

---

### 4. Calidad y Validación

#### 4.1 Testing
- Pruebas funcionales
- Validación requerimientos
- Corrección incidencias

#### 4.2 Validación Usuarios
- Validación operativa
- Retroalimentación usuarios
- Ajustes finales

---

### 5. Implementación y Cierre

#### 5.1 Despliegue
- Configuración servidor
- Publicación sistema
- Configuración productiva

#### 5.2 Capacitación
- Capacitación usuarios
- Manual usuario
- Soporte inicial

#### 5.3 Cierre Proyecto
- Entrega final
- Validación cliente
- Documentación cierre

---

## 4.2 Cronograma Simplificado

| Fase | Duración Estimada |
|---|---|
| Gestión y planificación | 2 semanas |
| Análisis y diseño | 3 semanas |
| Desarrollo plataforma SGII | 8 semanas |
| Calidad y validación | 2 semanas |
| Implementación y cierre | 2 semanas |

---

## 4.3 Dependencias Principales

- El diseño depende del levantamiento de requerimientos.
- El desarrollo depende de la arquitectura definida.
- Las pruebas dependen de la finalización del desarrollo.
- El despliegue depende de la validación funcional.
- El cierre depende de la aprobación del cliente.

---

## 4.4 Entregables Principales

- Documento de requerimientos.
- Diseño de arquitectura.
- Modelo de base de datos.
- Plataforma SGII funcional.
- Sistema de autenticación.
- Gestión de inventario.
- Gestión de ventas.
- Dashboard administrativo.
- Reportes y alertas.
- Manual técnico y usuario.
- Sistema desplegado.
---

# 5. Asignación de Roles y Recursos

## 5.1 Roles del Proyecto

| Rol | Responsabilidad Principal |
|---|---|
| Sponsor / Cliente | Aprobación general del proyecto y validación de entregables |
| Project Manager | Planificación, coordinación y seguimiento del proyecto |
| Product Owner | Priorización de requerimientos y validación funcional |
| Arquitecto de Software | Diseño de arquitectura y decisiones técnicas |
| Backend Developer | Desarrollo lógica de negocio y APIs |
| Frontend Developer | Desarrollo interfaz gráfica y experiencia de usuario |
| UX/UI Designer | Diseño visual y experiencia usuaria |
| QA Tester | Validación funcional y pruebas del sistema |
| DBA | Administración y modelado de base de datos |
| DevOps / Infraestructura | Configuración de servidores y despliegue |
| Especialista Seguridad | Validación de controles de seguridad y acceso |
| Usuarios Operativos | Retroalimentación funcional y pruebas operativas |

---

## 5.2 Recursos Humanos

### Equipo Base de Desarrollo
- 1 Project Manager
- 1 Product Owner
- 1 Arquitecto de Software
- 2 Software Developers
- 1 UX/UI Designer
- 1 QA Tester
- 1 DBA
- 1 DevOps

### Usuarios Participantes
- Administrador del Sistema
- Administrador de Bodega
- Vendedores

---

## 5.3 Recursos Tecnológicos

| Recurso | Uso Principal |
|---|---|
| Computadores de desarrollo | Construcción del sistema |
| Visual Studio Code | Desarrollo de software |
| GitHub | Control de versiones |
| Node.js | Backend |
| HTML/CSS/JavaScript | Frontend |
| MySQL/PostgreSQL | Base de datos |
| Servidor Cloud | Hosting y despliegue |
| Navegadores Web | Acceso al sistema |
| Herramientas de diseño UI | Diseño interfaces |
| Plataforma reuniones virtuales | Coordinación del equipo |

---

## 5.4 Recursos de Infraestructura

- Servidor de aplicación.
- Servidor de base de datos.
- Servicio de hosting cloud.
- Certificados SSL.
- Sistema de backups automáticos.
- Herramientas de monitoreo y logging.

---

## 5.5 Recursos Documentales

- Documento de requerimientos.
- Casos de uso.
- Diagramas UML.
- Documentación arquitectura.
- Manual técnico.
- Manual usuario.
- Planificación del proyecto.

---

## 5.6 Justificación de Recursos

Los recursos definidos permiten cubrir adecuadamente todas las áreas involucradas en el proyecto SGII, incluyendo planificación, diseño, desarrollo, pruebas, despliegue y soporte inicial.

La combinación de recursos humanos, tecnológicos y de infraestructura permite asegurar:
- desarrollo organizado,
- control de calidad,
- seguridad de la información,
- disponibilidad del sistema,
- mantenibilidad futura,
- correcta implementación operativa.

---

# 6. Matriz de Riesgos

## 6.1 Identificación y Evaluación de Riesgos

| Riesgo | Descripción | Impacto | Probabilidad | Estrategia de Mitigación | Responsable |
|---|---|---|---|---|---|
| Cambios frecuentes de requerimientos | Modificaciones constantes solicitadas durante el desarrollo pueden afectar tiempos y costos. | Alto | Alta | Validación temprana y control de cambios formal. | Project Manager |
| Errores de integridad en inventario | Inconsistencias de stock por fallos de lógica o concurrencia. | Alto | Media | Uso de transacciones, validaciones y pruebas integrales. | Arquitecto de Software |
| Accesos no autorizados | Usuarios podrían acceder a información o funciones restringidas. | Alto | Media | Implementación de autenticación segura y control por roles. | Especialista de Seguridad |
| Caída del servidor o indisponibilidad | Interrupción del sistema durante operaciones críticas. | Alto | Media | Monitoreo, backups y redundancia básica del servidor. | DevOps / Infraestructura |
| Pérdida o corrupción de datos | Fallos en la base de datos pueden afectar información crítica. | Alto | Baja | Backups automáticos y políticas de recuperación. | DBA |
| Retrasos en el desarrollo | Incumplimiento de fechas debido a sobrecarga o mala estimación. | Medio | Alta | Seguimiento semanal y planificación incremental. | Project Manager |
| Errores en despliegue productivo | Problemas durante publicación del sistema. | Medio | Media | Ambientes de prueba y checklist de despliegue. | DevOps |
| Baja adopción de usuarios | Resistencia al cambio o dificultad de uso del sistema. | Medio | Media | Capacitación y diseño centrado en el usuario. | Product Owner |
| Rendimiento insuficiente | Lentitud del sistema ante múltiples operaciones simultáneas. | Alto | Media | Optimización de consultas y pruebas de rendimiento. | Backend Developer |
| Dependencia de un integrante clave | Retrasos si un miembro crítico abandona o no está disponible. | Medio | Media | Documentación continua y distribución de conocimiento. | Project Manager |
| Errores funcionales en producción | Fallos detectados después de la implementación. | Alto | Media | Testing funcional y validación con usuarios. | QA Tester |
| Vulnerabilidades de seguridad | Posibles ataques o explotación de fallos de seguridad. | Alto | Baja | Validaciones, cifrado y revisión de seguridad periódica. | Especialista de Seguridad |

---

## 6.2 Estrategia General de Gestión de Riesgos

La gestión de riesgos del proyecto SGII se realizará de manera continua durante todo el ciclo de vida del proyecto, considerando:

- Identificación temprana de riesgos.
- Seguimiento periódico en reuniones de avance.
- Evaluación de impacto y probabilidad.
- Aplicación de medidas preventivas.
- Definición clara de responsables.
- Planes de contingencia para riesgos críticos.

---

## 6.3 Riesgos Prioritarios del Proyecto

Los riesgos considerados más críticos para el proyecto son:

1. Cambios frecuentes de requerimientos.
2. Errores de integridad del inventario.
3. Accesos no autorizados.
4. Caídas del sistema.
5. Retrasos en el desarrollo.

Estos riesgos requieren monitoreo constante debido a su impacto directo sobre:
- operación del negocio,
- continuidad del sistema,
- seguridad de la información,
- cumplimiento de plazos.

---

# 7. Selección de Metodología de Desarrollo

## 7.1 Propuesta Metodológica

Para el desarrollo del Sistema de Gestión de Inventario Inteligente (SGII) se propone utilizar un enfoque híbrido basado en PMI y Scrum.

La combinación de ambas metodologías permite equilibrar:
- planificación formal,
- control del proyecto,
- gestión de riesgos,
- adaptabilidad,
- desarrollo incremental,
- validación continua.

---

## 7.2 Justificación de PMI

PMI aporta una estructura formal de gestión del proyecto, permitiendo organizar adecuadamente:
- alcance,
- planificación,
- cronograma,
- recursos,
- riesgos,
- seguimiento.

### ¿Por qué se utiliza PMI en este proyecto?

El SGII involucra:
- múltiples entregables,
- distintos stakeholders,
- requerimientos técnicos y operacionales,
- coordinación de recursos,
- control de tiempos y riesgos.

Debido a esto, se requiere una metodología que permita mantener control y trazabilidad sobre todo el ciclo de vida del proyecto.

### Beneficios de PMI para el SGII

- Mejor organización del proyecto.
- Control formal del alcance.
- Gestión estructurada de riesgos.
- Seguimiento del cronograma.
- Definición clara de roles y responsabilidades.
- Mejor comunicación con stakeholders.

---

## 7.3 Justificación de Scrum

Scrum se utilizará como metodología ágil para la etapa de desarrollo e implementación del software.

### ¿Por qué se utiliza Scrum?

El proyecto SGII puede requerir:
- ajustes funcionales,
- retroalimentación constante,
- mejoras progresivas,
- validaciones operativas continuas.

Scrum permite adaptarse rápidamente a cambios y entregar funcionalidades de forma incremental.

### Beneficios de Scrum para el SGII

- Entregas parciales funcionales.
- Validación temprana con usuarios.
- Mayor flexibilidad frente a cambios.
- Retroalimentación continua.
- Detección temprana de errores.
- Mejor colaboración del equipo.

---

## 7.4 Estrategia de Trabajo

La estrategia del proyecto combinará control administrativo mediante PMI y ejecución iterativa mediante Scrum.

### Estrategia General

- Planificación inicial utilizando lineamientos PMI.
- Definición de alcance, riesgos y cronograma.
- Desarrollo incremental mediante Sprints Scrum.
- Validación funcional continua con usuarios.
- Seguimiento periódico del avance.

---

## 7.5 Implementación de Scrum

### Sprint

Se trabajará con Sprints de 2 semanas para entregar funcionalidades progresivas del SGII.

### Product Backlog

El Product Backlog contendrá:
- requerimientos funcionales,
- mejoras,
- incidencias,
- tareas técnicas.

### Sprint Planning

En cada Sprint se seleccionarán las funcionalidades prioritarias a desarrollar.

### Daily Scrum

Reuniones breves diarias para:
- revisar avances,
- identificar bloqueos,
- coordinar tareas.

### Sprint Review

Validación funcional con stakeholders y usuarios clave.

### Sprint Retrospective

Evaluación interna del equipo para identificar mejoras en el proceso de trabajo.

---

## 7.6 Roles Scrum

| Rol | Responsabilidad |
|---|---|
| Product Owner | Priorizar requerimientos y validar funcionalidades |
| Scrum Master | Facilitar metodología y eliminar impedimentos |
| Equipo de Desarrollo | Construcción técnica del sistema |
| Stakeholders | Retroalimentación y validación operativa |

---

## 7.7 Estrategia de Seguimiento y Control

Para asegurar el correcto avance del proyecto se utilizarán:

- reuniones semanales de seguimiento,
- revisión de avances por Sprint,
- control de riesgos,
- control de cambios,
- métricas de cumplimiento,
- validación continua de entregables.

---

## 7.8 Resultado Esperado

La utilización de un enfoque híbrido PMI + Scrum permitirá:

- mantener control organizacional,
- adaptarse a cambios funcionales,
- mejorar la calidad del software,
- reducir riesgos,
- entregar valor progresivamente,
- facilitar la comunicación entre las partes involucradas.

---

# 8. Plan de Comunicación

| Actividad de Comunicación | Participantes | Medio | Frecuencia | Objetivo |
|---|---|---|---|---|
| Kickoff del Proyecto | Sponsor, PM, Equipo | Reunión presencial/virtual | Inicio del proyecto | Presentar objetivos, alcance y organización del proyecto |
| Daily Scrum | Equipo de desarrollo | Reunión breve | Diario | Coordinar tareas y detectar bloqueos |
| Reunión de Seguimiento | PM y equipo técnico | Meet / Teams | Semanal | Revisar avances, riesgos y cumplimiento |
| Sprint Planning | Product Owner y equipo | Reunión virtual | Cada Sprint | Definir tareas y objetivos del Sprint |
| Sprint Review | Stakeholders y equipo | Presentación funcional | Cada Sprint | Validar funcionalidades implementadas |
| Reporte de Avance | PM → Gerencia | Correo / Documento | Quincenal | Informar estado general del proyecto |
| Gestión de Incidencias | Equipo técnico | Plataforma colaborativa | Permanente | Reportar y resolver problemas técnicos |
| Validación con Usuarios | Usuarios clave y equipo | Reunión / Demo | Según avance | Obtener retroalimentación funcional |
| Comité Ejecutivo | Sponsor y PM | Reunión ejecutiva | Mensual | Revisar cumplimiento estratégico |
| Cierre del Proyecto | Todos los stakeholders | Reunión final | Fin del proyecto | Presentar entregables y cierre formal |

---

# 9. Cierre de Proyecto y Transición

## 9.1 Entregables Finales

Al finalizar el proyecto se entregarán los siguientes componentes asociados al Sistema de Gestión de Inventario Inteligente (SGII):

- Plataforma SGII completamente operativa.
- Sistema de gestión de inventario.
- Sistema de registro de ventas.
- Gestión de usuarios y roles.
- Sistema de auditoría y trazabilidad.
- Alertas automáticas de stock crítico.
- Reportes operacionales.
- Base de datos configurada.
- Código fuente documentado.
- Manual técnico.
- Manual de usuario.
- Documentación de arquitectura.
- Configuración de despliegue e infraestructura.

---

## 9.2 Criterios de Aceptación

El proyecto será considerado aceptado cuando se cumplan los siguientes criterios:

- El sistema registra ventas correctamente.
- El inventario se actualiza en tiempo real.
- Los usuarios acceden según sus permisos y roles.
- Las alertas de stock funcionan correctamente.
- La auditoría registra las acciones relevantes.
- El sistema mantiene estabilidad operativa.
- Los requerimientos funcionales críticos fueron implementados.
- Los stakeholders validan el funcionamiento esperado.
- La documentación fue entregada correctamente.

---

## 9.3 Actividades de Transición

Durante la etapa de transición se ejecutarán las siguientes actividades:

| Actividad | Objetivo |
|---|---|
| Capacitación de usuarios | Facilitar el uso correcto del sistema |
| Implementación en producción | Publicar el sistema en ambiente operativo |
| Configuración inicial | Ajustar parámetros y usuarios iniciales |
| Migración de datos | Incorporar información necesaria al sistema |
| Validación operativa | Confirmar correcto funcionamiento en producción |
| Soporte inicial | Resolver incidencias posteriores al despliegue |

---

## 9.4 Estrategia de Soporte Inicial

Después de la implementación se considerará un período de soporte inicial para:

- corrección de errores,
- ajustes menores,
- resolución de incidencias,
- apoyo a usuarios,
- monitoreo del sistema.

El soporte permitirá asegurar estabilidad y adaptación adecuada durante el inicio de operación del SGII.

---

## 9.5 Cierre Administrativo del Proyecto

El cierre administrativo contemplará:

- aprobación formal del cliente,
- validación de entregables,
- cierre documental,
- respaldo de información del proyecto,
- consolidación de lecciones aprendidas,
- cierre contractual y organizacional.

---

## 9.6 Lecciones Aprendidas Esperadas

Durante el desarrollo del SGII se espera identificar oportunidades de mejora relacionadas con:

- gestión de inventario digital,
- coordinación del equipo,
- validación temprana,
- control de riesgos,
- automatización de procesos,
- seguridad y trazabilidad de información.

Estas lecciones permitirán mejorar futuros proyectos tecnológicos similares.

---

## 9.7 Métricas Organizacionales Impactadas

La implementación del Sistema de Gestión de Inventario Inteligente (SGII) impactará directamente distintas métricas operacionales y organizacionales relacionadas con eficiencia, control y calidad del servicio.

| Métrica | Impacto Esperado |
|---|---|
| Reducción de errores de inventario | Disminución de inconsistencias y diferencias de stock |
| Tiempo de actualización de inventario | Actualización inmediata de movimientos y ventas |
| Tiempo de registro de ventas | Procesos de venta más rápidos y eficientes |
| Disponibilidad de información | Acceso en tiempo real a datos operacionales |
| Nivel de trazabilidad | Mayor control sobre movimientos y acciones realizadas |
| Incidentes por accesos indebidos | Disminución mediante control de roles y permisos |
| Tiempo de respuesta del sistema | Mejor rendimiento en operaciones críticas |
| Nivel de satisfacción de usuarios | Mejora en experiencia de uso y operación diaria |
| Gestión de stock crítico | Disminución de quiebres de stock |
| Tiempo de generación de reportes | Automatización y acceso rápido a información |
| Continuidad operacional | Mayor estabilidad y disponibilidad del sistema |
| Eficiencia operativa | Optimización de procesos administrativos y de inventario |