# Base de Datos para un Concesionario de Vehículos

## Descripción del Proyecto

Este proyecto consiste en el diseño de una base de datos para un concesionario de vehículos, permitiendo gestionar la información sobre los vehículos en stock, clientes, ventas y servicios de mantenimiento. La base de datos facilita el registro y administración de:

- 🚗 **Vehículos disponibles en inventario**
- 👤 **Clientes y su historial de compras y servicios**
- 👨‍💼 **Vendedores y sus transacciones de ventas**
- 💰 **Registro de ventas y métodos de pago**
- 🛠️ **Servicios de mantenimiento realizados a los vehículos**

## 📌 DIAGRAMAS Y SQL:

https://probable-cosmonaut-fb2.notion.site/Examen-Introducci-n-al-backend-1a81c5deb11080e09f05f911f7346a1a


## 🔗 Relaciones y Restricciones

- **idVeh** es clave primaria en la tabla **vehiculo** y debe ser **único**.
- Cada **venta** está asociada a un **cliente** (**idCliente**) y un **vendedor** (**idVend**).
- Un **vehículo vendido cambia su estado a "no disponible" en el inventario**.
- Se aplican **claves foráneas** para garantizar la **integridad referencial** entre tablas.

## 📖 Justificación del Diseño

El diseño de esta base de datos permite:

✅ **Eficiente almacenamiento y recuperación de información clave.**
✅ **Relacionar adecuadamente los elementos para un mejor control del inventario, ventas y servicios.**
✅ **Mantener integridad de datos con restricciones como claves primarias y foráneas.**
✅ **Facilitar el seguimiento de historial de ventas y mantenimiento de cada vehículo.**

## ⚠️ Restricciones y Validaciones

- 🔹 **Claves primarias y foráneas establecidas** para evitar datos inconsistentes.
- 🔹 **Validación de unicidad en VIN** (**numSerie**) para evitar duplicados.
- 🔹 **Restricción en disponibilidad de vehículos vendidos.**
- 🔹 **Uso de valores booleanos** para estado y disponibilidad.

