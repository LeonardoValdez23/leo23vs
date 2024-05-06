# Autómata Finito en Máquina Expendedora de Bebidas

Ejemplo de aplicación de un autómata finito en el diseño de un sistema de control para una máquina expendedora de bebidas en un establecimiento.


![Diagrama](/Imagenes-tema-3/maquina-ex2.png)


## Aplicación del autómata finito

El autómata finito se utiliza para modelar el comportamiento de la máquina expendedora, incluyendo sus diferentes estados y las transiciones entre ellos en respuesta a eventos específicos.

### Estados del autómata

- **Esperando Moneda:** La máquina está esperando que se inserte la cantidad correcta de monedas para poder seleccionar un producto.
- **Seleccionando Producto:** Una vez se ha insertado la moneda necesaria, el usuario puede seleccionar un producto de la máquina.
- **Entregando Producto:** Después de la selección, la máquina procede a entregar el producto al usuario.
- **Reiniciando:** En caso de errores o falta de inventario, la máquina puede pasar al estado de reinicio para restablecer su funcionamiento.

### Transiciones entre estados

- **Insertar Moneda:** Activada al insertar la cantidad correcta de monedas, lleva de "Esperando Moneda" a "Seleccionando Producto".
- **Seleccionar Producto:** Activada al elegir un producto, lleva de "Seleccionando Producto" a "Entregando Producto".
- **Entregar Producto:** Activada al completar la entrega del producto, lleva de "Entregando Producto" a "Esperando Moneda" para la siguiente transacción.
- **Reiniciar:** Activada en caso de errores, lleva a la máquina al estado de "Reiniciando" para solucionar problemas.

## Diagrama de Estados y Transiciones
![Diagrama](/Imagenes-tema-3/maquina-expendedora.png)


