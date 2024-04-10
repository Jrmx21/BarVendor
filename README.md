# BarVendor
# Temática
Mi proyecto se trata de una aplicación web y una aplicación móvil para realizar pedidos en bares y registrar las ventas. Por un lado la aplicación web que tendrá acceso al apartado administrativo donde podrás configurar la base de datos mediante CRUD y una aplicación móvil con la que el camarero podrá realizar pedidos y que lleguen a cocina y a barra.

# Perfiles de usuario:
Habrán 3 perfiles de usuarios, administradores y cocina con el acceso total a toda la interfaz de aplicación web y gestor que podrá realizar algunas acciones de vista en las bases de datos como ver el plato más vendido.
Por otro lado estará el móvil/tablet del camarero como tipo de perfil de usuario único de la aplicación Ionic.
Épicas de la aplicación
El sistema realizará CRUD sobre una base de datos consistente que tendrá las siguientes tablas:
Usuarios(con los roles predefinidos)
Productos(Estarán organizados por categoria: platos,bebidas, entrantes… Esta tabla tendrá el precio con el IVA aplicado)
Cuentas (se meterán también en pedidos en curso)
Facturas (registrando la fecha y el pedido, en esta tabla se acumularán todos los pedidos de una mesa hasta que se sienten otros comensales habiendo pagado los anteriores,)
Mesas(serán todas las mesas del bar/restaurante)
Pedidos(Todos los pedidos que se han realizado con una propiedad booleana que es true si el pedido ha sido servido y false si no. Tendrá como clave foránea el id usuario, el id mesa y id de producto)
El usuario gestor podrá aplicar descuento desde la aplicación web en los platos para poder llamar la atención de nuevos clientes(operación transaccional).

Y por el otro lado en aplicación móvil, realizará pedidos con notas de los comensales(Por ejemplo:carne muy hecha, poco hecha…) que anotará el camarero.
