# Microservicios-GestionPedidos

## Servicio de Gestión de Pedidos

### Contexto del Proyecto

En la era del comercio electrónico, la gestión eficiente de los pedidos es crucial para brindar una experiencia satisfactoria al cliente. Este proyecto es un **microservicio de gestión de pedidos** desarrollado en **.NET 8** con **Entity Framework Core** y **Docker**. El objetivo es proporcionar un sistema escalable y mantenible que permita a las empresas gestionar los pedidos de manera efectiva.

### Beneficios

- **Escalabilidad**: Gracias a la arquitectura de microservicios, cada componente del sistema puede escalar de manera independiente, lo que permite un uso eficiente de los recursos.
- **Mantenibilidad**: La separación de preocupaciones facilita la gestión y el mantenimiento del código, permitiendo a los desarrolladores trabajar en diferentes microservicios sin interferir entre sí.
- **Resiliencia**: La comunicación asincrónica a través de **RabbitMQ** permite que los microservicios sigan funcionando incluso si uno de ellos falla, mejorando la robustez del sistema.

### Funcionalidades

1. **Gestión de Pedidos**: 
   - Creación de nuevos pedidos.
   - Lectura de detalles de pedidos existentes.
   - Actualización del estado de los pedidos.
   - Eliminación de pedidos.

2. **Gestión de Clientes**:
   - Creación y gestión de perfiles de clientes.
   - Historial de pedidos de los clientes.

3. **Gestión de Inventario**:
   - Control de stock de productos.
   - Actualización automática del inventario tras la creación de un pedido.

4. **Notificaciones**:
   - Envío de notificaciones al cliente sobre el estado del pedido (confirmación, envío, entrega).

### Componentes de la Arquitectura

La arquitectura del proyecto incluye los siguientes componentes:

- **Microservicio de Gestión de Pedidos**: 
  - Encargado de la lógica de negocio relacionada con los pedidos.
  - Comunica con otros microservicios (clientes, inventario) a través de **RabbitMQ**.

- **Microservicio de Gestión de Clientes**:
  - Maneja la información de los clientes y sus interacciones con los pedidos.

- **Microservicio de Gestión de Inventario**:
  - Controla la disponibilidad de productos y su stock.

- **Microservicio de Notificaciones**:
  - Envía alertas y actualizaciones a los clientes sobre el estado de sus pedidos.

- **RabbitMQ**:
  - Broker de mensajes utilizado para la comunicación entre microservicios, permitiendo un flujo de información eficiente y desacoplado.

- **Base de Datos**:
  - SQL Server se utiliza para almacenar de manera persistente la información de pedidos, clientes e inventario.

- **Azure**:
  - Plataforma en la nube para el despliegue y gestión de recursos, proporcionando un entorno robusto para los microservicios.

### Tecnologías Utilizadas

- **Lenguaje**: C#
- **Framework**: .NET 8
- **ORM**: Entity Framework Core
- **Base de Datos**: SQL Server
- **Mensajería**: RabbitMQ
- **Plataforma en la Nube**: Microsoft Azure
- **Contenerización**: Docker

### Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/Microservicios-GestionPedidos.git
   cd Microservicios-GestionPedidos
