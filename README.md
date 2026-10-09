# Diagrama-de-Calles-Carrito-Liverpool
Creadores: Brandon Isaac Miranda Montes, Juraz Gael Miranda Coronado y Erick Bustamante Cruz


Trabajo escolar sobre carritos digitales (elegimos Liverpool). Realizamos un diagrama de calles (o secuencia) que detalla cada acción del proceso de compra: desde buscar un producto en la tienda web, hasta finalizar la transacción y revisar el estado del pedido paso a paso.

![Diagrama del carrito de Liverpool](<Diagrama carrito Liverpool.jpg>)


### Explicación del Flujo de Compra

Este diagrama de calles modela el proceso completo de compra en Liverpool, dividiendo las acciones entre cuatro actores principales: **Cliente, Carrito, Inventario y Banco**.

El flujo se divide en las siguientes etapas clave:

1. **Selección de Productos:** El cliente busca y agrega productos. El sistema consulta en tiempo real con el inventario para validar la disponibilidad (stock) antes de añadirlo y calcular el subtotal.
2. **Edición del Carrito:** El cliente puede modificar las cantidades o eliminar productos. Cualquier cambio actualiza automáticamente tanto el subtotal como las existencias apartadas en el inventario.
3. **Autenticación y Envío:** Para proceder al pago, se requiere iniciar sesión. El inventario hace una reevaluación final de stock y el cliente elige su método de entrega ("Click & Collect" o envío a domicilio).
4. **Proceso de Pago:** El cliente selecciona su método de pago (Tarjeta, PayPal, Efectivo). Aquí interviene el Banco para validar la forma de pago y comprobar que existan fondos suficientes.
5. **Confirmación del Pedido:** Una vez aprobado el pago, el sistema genera la orden de compra, envía los correos de confirmación y el ticket, vacía el carrito virtual y proporciona un enlace para el rastreo del paquete.
