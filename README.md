# Sistema de Gestión de Base de Datos para Retail (Ferretería) 

Este proyecto consiste en el diseño e implementación de una base de datos relacional robusta para gestionar el inventario, facturación y clientes de una ferretería de alto volumen.

## Objetivo
Simular un entorno de producción donde la integridad de los datos y la velocidad de consulta son críticos. El proyecto se centra en la normalización, el uso de procedimientos almacenados para la lógica de negocio y la optimización mediante índices.

## Tecnologías Utilizadas
* **Motor:** Microsoft SQL Server
* **Lenguaje:** T-SQL (Transact-SQL)
* **Scripting:** Python (para pruebas de carga y estrés)

## Características Destacadas
* **Arquitectura Relacional:** Diseño normalizado (3NF) para evitar redundancia.
* **Integridad de Datos:** Implementación estricta de `FOREIGN KEYS` y `CHECK CONSTRAINTS` para validar inventarios negativos y tipos de datos.
* **Lógica de Negocio:** Uso de **Stored Procedures** para transacciones complejas (ej. "Generar Factura" que descuenta stock automáticamente).
* **Optimización:** Estrategia de indexación (**Clustered** vs **Non-Clustered**) aplicada a campos de búsqueda frecuente como `Fecha_Factura` y `ID_Cliente`.
* **Seguridad y Mantenimiento:** Scripts configurados para copias de seguridad (Backups) y auditoría básica.

##  Integración con Python
Se incluyen scripts en Python para realizar inserciones masivas de datos de prueba y validar el comportamiento de la base de datos bajo carga.
