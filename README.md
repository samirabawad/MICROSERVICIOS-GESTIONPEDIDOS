# MICROSERVICIOS-GESTIONPEDIDOS
Microservicio de gestión de pedidos, desarrollado en .NET 8 con Entity Framework Core y Docker. Este proyecto incluye múltiples microservicios para gestionar pedidos, clientes, inventario y notificaciones, utilizando RabbitMQ para la comunicación entre servicios.

# Servicio de Gestion de Pedidos

## Descripción del Proyecto

Este proyecto es un **microservicio de gestión de pedidos** desarrollado en **.NET 8** con **Entity Framework Core**. El servicio permite crear, leer, actualizar y eliminar pedidos en un sistema de comercio electrónico, facilitando la gestión eficiente de la información de pedidos.

### Características

- **Gestión de Pedidos**: Permite realizar operaciones CRUD sobre los pedidos.
- **Comunicación Asincrónica**: Utiliza **Kafka** para la comunicación entre microservicios, asegurando un sistema desacoplado y escalable.
- **Despliegue en la Nube**: Integración con **Azure** para el despliegue y gestión de recursos.

### Tecnologías Utilizadas

- **Lenguaje**: C#
- **Framework**: .NET 8
- **ORM**: Entity Framework Core
- **Base de Datos**: SQL Server
- **Mensajería**: Apache Kafka o Azure Event Hubs
- **Plataforma en la Nube**: Microsoft Azure

### Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/OrderManagementService.git
   cd OrderManagementService
