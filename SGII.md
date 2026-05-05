# Sistema de Gestión de Inventario Inteligente (SGII)

## Contexto

Sistema web para control de inventario en tiempo real para una cadena de tiendas minoristas.  
Busca disminuir quiebres de stock, mejorar la trazabilidad de productos y automatizar procesos de reposición.

---

## A. Concepción

### Preguntas iniciales

- **¿Qué problema resuelve el sistema?**  
  **Respuesta:** El sistema resuelve el problema del control manual o parcialmente digital del inventario, que genera errores humanos, pérdidas de stock y retrasos en la reposición.

- **¿Quién registra entradas y salidas de productos? ¿Quién gestiona el inventario?**  
  **Respuesta:** El Administrador de Bodega (**Actor**) registra entradas y gestiona inventario. El Vendedor registra salidas mediante ventas.

- **¿Cuántas sucursales considera el sistema inicialmente?**  
  **Respuesta:** Inicialmente 1 sucursal, con posibilidad de escalar a múltiples sucursales.

- **¿Cuáles son los horarios operacionales del sistema?**  
  **Respuesta:** Horario comercial (ej. 09:00 a 18:00), con disponibilidad esperada del sistema de 99.9%.

- **¿Qué tipos de productos existen?**  
  **Respuesta:** Productos de inventario minorista organizados por categorías.

- **Cuando se menciona control de inventario, ¿existe actualmente un sistema o es manual?**  
  **Respuesta:** Actualmente el proceso es parcialmente manual.

- **¿Realizar algún tipo de reporte?**
  **Respuesta:** Sí, reportes de stock crítico, movimientos de inventario y ventas por período.

- **Aparte del vendedor y administrador, ¿quién más interactúa con el sistema?**  
  **Respuesta:** Un sistema externo de proveedores que recibe órdenes automáticas de reposición.

### Objetivo de esta actividad

Obtener los actores, los casos de uso principales y determinar si existen restricciones o reglas de negocio importantes. Obtener una vista preliminar del alcance del sistema a desarrollar.

---

## B. Indagación

### Actividades

- Paso 1: Capturar detalles sobre las funcionalidades descritas:
    - ¿Cómo funciona el registro de entradas de productos?
    - ¿Cómo se registra una venta?
    - ¿Cómo se valida disponibilidad de stock?
    - ¿Qué reglas existen para reposición automática?
    - ¿Qué notificaciones se deben generar?
    - ¿Qué reportes requiere administración?

- Paso 2: Obtener números iniciales:
  - Número de productos: ~1.000
  - Movimientos diarios: 150–300
  - Usuarios simultáneos: 5–10
  - Historial por producto: múltiples registros

- Paso 3: Identificar roles o tipos de usuarios:

  - Administrador del sistema: Configura usuarios, roles y parámetros
  - Administrador de bodega: Controla inventario y registra entradas
  - Vendedor: Realiza ventas y consulta stock
  - Sistema de proveedores: Recibe órdenes automáticas

- Paso 4: Definir qué debe hacer o no hacer cada rol.

- Paso 5: Identificar sistemas externos que se integran:
  - Sistema de proveedores
  - Sistema POS (futuro)

- Paso 6: Otro aspecto relevante:
  - Auditoría de movimientos
  - Seguridad por roles
  - Trazabilidad completa

### Objetivo de la actividad

Generar conclusiones y recomendaciones para el usuario. Obtener un alcance del software más cercano.

### Ejemplo de recomendación

Recomendamos poner foco en el control de inventario en tiempo real para resolver el problema principal.  

Esto implica considerar:

- Autenticación
- Autorización (roles)
- Trazabilidad de movimientos
- Funciones:
  - Registrar entrada
  - Registrar venta
  - Actualizar inventario
- Alertas automáticas
- Órdenes automáticas a proveedores

---

## C. Actores / Usuarios

Enumerar y detallar cada uno.

1. Administrador del sistema  
2. Administrador de bodega  
3. Vendedor  
4. Sistema de proveedores  

---

## D. Casos de Uso

### Casos de uso del vendedor

- **CU1:** Realizar venta  
- **CU2:** Consultar disponibilidad  

### Casos de uso del administrador de bodega

- **CU3:** Registrar entrada de mercadería  
- **CU4:** Actualizar inventario  
- **CU5:** Revisar historial  

### Casos de uso del administrador del sistema

- **CU6:** Gestionar usuarios  
- **CU7:** Configurar roles  
- **CU8:** Configurar parámetros  

### Casos de uso automatizados del sistema

- **CU9:** Generar alertas automáticas  
- **CU10:** Generar orden automática a proveedores  

---

## E. Reglas de Negocio

- **RN1:** No se puede vender sin stock disponible  
- **RN2:** Toda entrada debe estar respaldada por documento  
- **RN3:** El sistema debe generar alertas al alcanzar stock mínimo  
- **RN4:** Todo movimiento debe quedar registrado  
- **RN5:** Solo usuarios autorizados pueden modificar inventario  

---

## F. Requerimientos No Funcionales

### Seguridad

- **RNF1:** El sistema debe proveer autenticación y autorización  
- **RNF2:** El sistema debe registrar auditoría de accesos  

### Disponibilidad

- **RNF3:** Disponibilidad > 99,9% en horario laboral  

### Rendimiento

- **RNF4:** Respuesta < 100 ms en operaciones estándar  

### Usabilidad

- **RNF5:** Mostrar mensajes claros ante errores  
- **RNF6:** Máximo 3 pasos para registrar una venta  
- **RNF7:** Interfaz simple para consulta de stock  

---

## G. Priorización QFD + (Método MoSCoW)

### 1. Requerimientos Normales

- **CU1:** Realizar venta (**Must**)  
- **CU2:** Consultar disponibilidad (**Must**)  
- **CU3:** Registrar entrada (**Must**)  

### 2. Requerimientos Esperados

- **CU4:** Actualizar inventario (**Must**)  
- **CU5:** Revisar historial (**Should**)  

### 3. Requerimientos Emocionantes

- **CU9:** Alertas automáticas (**Could**)  
- **CU10:** Orden automática (**Could**)  

---

### Tabla de trazabilidad

| Necesidad del usuario | Requerimiento del sistema | Tipo DFC | Prioridad (MoSCoW) |
|---|---|---|---|
| Registrar ventas rápidamente | CU1 | Normal | Must |
| Consultar stock en tiempo real | CU2 | Normal | Must |
| Registrar entradas | CU3 | Normal | Must |
| Mantener inventario actualizado | CU4 | Esperado | Must |
| Revisar historial | CU5 | Esperado | Should |
| Recibir alertas | CU9 | Emocionante | Could |

---

## H. Criterios de Aceptación

### CU1: Realizar venta (**Must**)

- **CA1**
  - **Given:** el vendedor selecciona un producto  
  - **When:** el stock es insuficiente  
  - **Then:** el sistema bloquea la venta  

- **CA2**
  - **Given:** existe stock disponible  
  - **When:** se confirma la venta  
  - **Then:** el sistema descuenta stock automáticamente  

### CU3: Registrar entrada (**Must**)

- **CA1**
  - **Given:** el administrador registra un producto  
  - **When:** ingresa cantidad válida  
  - **Then:** el sistema actualiza el inventario  

### CU9: Generar alerta (**Could**)

- **CA1**
  - **Given:** el stock está bajo el mínimo  
  - **When:** el sistema detecta la condición  
  - **Then:** genera una alerta automática  

---