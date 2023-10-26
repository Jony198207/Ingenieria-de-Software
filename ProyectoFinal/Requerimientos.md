# Especificación de Requerimientos

## Tabla de Contenidos

* [Introduccion](##introduccion)
* [Descripción](##descripción)
* [System Features](##system-features)

## Introducción

Los requerimientos defienen los elementos indispensables para que una página web de una cafetería que ofrece solo bebidas pueda operar satisfactoriamente. En función del cumplimiento de los requerimientos es que el proyecto se definirá como exitoso, dado que estos reflejan las necesidades demandadas por el cliente con respecto al producto. 

## Descripción

### Perspectivas del producto 

La aplicación de la cafetería se centrará en proporcionar a los clientes una experiencia completa y conveniente. Incluirá un menú digital interactivo con opciones de personalización, permitirá pedidos en línea con pagos seguros, e implementará un programa de lealtad con descuentos y promociones exclusivas. 


## System Features

## Iniciar sesión

Para acceder a su cuenta, el usuario realiza el inicio de sesión ingresando su nombre de usuario y contraseña, los cuales previamente ha registrado en el sistema.

> **High Priority**: Este requisito es esencial para obtener las credenciales de los clientes, permitiendo así el procesamiento eficiente de sus pedidos.

#### Secuencia de respuesta y requerimientos funcionales

* *buttons*: Log in, Sign up
* *textBox*: nombre del usuario y contraseña


### Seleccionar y procesar método de pago

El usuario puede elegir entre los distintos métodos de pago disponibles: débito, crédito y efectivo. Posteriormente, se deben llenar los datos correspondientes al método elegido, tales como información de la tarjeta. En caso de ser efectivo, se debe calcular el cambio necesario para que sea entregado por el repartidor durante la entrega a domicilio. Una vez recibida esta información, se procesa el pago, para autorizar la preparación y envío del producto.

> **High Priority**: con este requerimiento recibimos ingresos, lo que permite al negocio continuar en servicio

#### Secuencia de respuesta y requerimientos funcionales

Una vez que el usuario termine de llenar su carrito, oprime el botón de 'pagar'. En el pago debe haber links con imágenes hacia las distintas opciones. Según el tipo de opción, deberan aparecer pestañas para llenar la información correspondiente. Posteriormente, se hace el procesamiento y se acepta o no el pago. En caso de ser rechazado, se debe repetir el proceso desde la selección de un método.
* *buttons*: iniciar pago, seleccionar método, finalizar pago
* *dropDownList*: fecha de caducidad
* *textBox*: nombre en la tarjeta, codigo de seguridad (en modo contraseña)

### Personalizar bebida

El usuario puede añadir un toque personalizado a su bebida al poder definir: tamaño, crema batida, shots de café adicionales, toppings de crema batida, tipo de leche, número de endulzantes, entre otros. Según el tipo de bebida, ciertas opciones no estarán disponibles; por ejemplo, las bebidas calientes no acostumbran llevar crema batida. 

> **High Priority**: hoy en día, es muy importante tener la capacidad de adaptar nuestros productos a las preferencias del consumidor, y así, ofrecer una gran experiencia

#### Secuencia de respuesta y requerimientos funcionales

Cuando el usuario termine de seleccionar su bebida, se debe abrir una pestaña con los opciones de personalización. El usuario dará click según sus preferencias y agregará el producto a su carrito. En caso de no seleccionar una opción, se tomará en cuenta el valor default definido por la cafeteria.
* *radioButtons*: permiten una selección rápida y restringen las opciones a lo establecido por la cafeteria

### Reseñas y calificaciones de bebidas

Los usuarios tienen la opción de dejar reseñas y calificaciones para las bebidas que han ordenado. Esta funcionalidad proporciona retroalimentación valiosa tanto para la cafetería como para otros clientes potenciales. Las reseñas pueden incluir comentarios sobre el sabor, la presentación y cualquier personalización específica realizada.

> **Medium Priority**: Agregar esta función puede mejorar la confianza del cliente y ayudar a promocionar las bebidas más populares.

#### Secuencia de respuesta y requerimientos funcionales

Después de completar un pedido, el usuario tiene la opción de dejar una reseña y asignar una calificación a la bebida en una escala de 1 a 5 estrellas. También puede escribir comentarios adicionales para proporcionar detalles específicos sobre su experiencia. Estas reseñas estarán disponibles para que otros clientes las vean al explorar el menú.

* *starsRating*: Permite a los usuarios asignar fácilmente una calificación a la bebida.
* *textBox*: Espacio para que los usuarios ingresen comentarios adicionales.
* *button*: Enviar reseña.

### Destacar Bebidas Populares

En la página principal, se destacarán las bebidas más populares basadas en las calificaciones y reseñas de los usuarios. Esto ayuda a los nuevos clientes a descubrir las opciones más apreciadas y contribuye a la promoción de productos destacados.

> **Low Priority**: Aunque no es de alta prioridad, resaltar las bebidas populares puede influir positivamente en las decisiones de compra.

#### Secuencia de respuesta y requerimientos funcionales

En la sección principal del menú, se mostrarán las bebidas mejor calificadas y más comentadas, junto con sus respectivas calificaciones y comentarios. Estas recomendaciones se actualizarán dinámicamente según las nuevas reseñas y calificaciones recibidas.

* *updates*: Automatización para actualizar las recomendaciones basadas en las nuevas reseñas.

### Programa de Recompensas

La cafetería implementará un programa de recompensas para fomentar la lealtad del cliente. Los usuarios acumularán puntos por cada compra realizada a través de la plataforma en línea. Estos puntos podrán canjearse por descuentos, productos gratuitos u otras recompensas especiales.

> **High Priority**: La implementación de un programa de recompensas puede incentivar a los clientes a realizar pedidos recurrentes y aumentar la retención.

#### Secuencia de respuesta y requerimientos funcionales

Cada vez que un usuario realiza un pedido, acumula puntos en su cuenta. Los puntos acumulados se mostrarán en la interfaz del usuario, y se proporcionará una descripción clara de las recompensas disponibles y cómo pueden canjearse. Los clientes podrán aplicar sus puntos durante el proceso de pago para obtener descuentos o recompensas específicas.

* *Tracker de puntos*: Sistema de seguimiento de puntos acumulados.
* *Catálogo de recompensas*: Catálogo que muestra las recompensas disponibles dependiendo de la temporada del año o existencia de las recompensas.




