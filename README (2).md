# Actividad Práctica – AEE

## Modelado de Comportamiento en Sistemas de E-commerce

Hemos realizado el diagrama siguiendo un proceso de compra, en el que comienza con un punto negro para poder dar comiendo a la primera acción en el “pulsar finalizar compra”, luego hemos utilizado un flujo de actividades en paralelo en el que dentro existe la opción de revisar stock y validar sesión, es decir, que se hacen simultáneamente. 

Luego dependiendo de las posibilidades de stock, según si hay o no puede finalizar o continuar a la fase de pedir los datos de la compra. Luego utilizamos otro flujo de actividades en paralelo, ya que se hace simultáneamente todo el proceso de relleno de datos de la tarjeta. Posteriormente se validan los datos de la tarjeta, y de nuevo se marcan la posibilidad de dos opciones, si la tarjeta no es válida manda un mensaje de error, de ahí puesto el círculo con X debido a que por ese camino finaliza pero los demás procesos siguen funcionando, y si la tarjeta es válida continúa el proceso de compra.

En el proceso de facturación, continuando lo anterior, hemos vuelto a utilizar un flujo de actividades en paralelo debido a que se hacen simultáneamente, la generación del PDF de la factura, el registro del pedido en la base de datos, y por último el envío de una notificación por correo, y posteriormente se manda un mensaje de confirmación para finalizar.

<img width="576" height="647" alt="image" src="https://github.com/user-attachments/assets/ed6d4e36-721c-4e61-a531-9f17a856734a" />
