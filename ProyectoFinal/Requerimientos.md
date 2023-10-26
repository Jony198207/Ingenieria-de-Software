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




