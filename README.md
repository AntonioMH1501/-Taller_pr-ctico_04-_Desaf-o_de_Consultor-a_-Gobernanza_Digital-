# -Taller_pr-ctico_04-_Desaf-o_de_Consultor-a_-Gobernanza_Digital-

## Análisis de Mercado y Selección
Bloque A
Hemos elegido Odoo, basándonos en el perfil de la empresa con 25 empleados, presupuesto ajustado y necesidad de personalización en el etiquetado. La elección de esta plataforma se debe a que la empresa cuenta con un presupuesto limitado, ya que Odoo es Open Source y este presupuesto se podría redirigir a otros sectores. Está act

La empresa que nos ha contratado, "Aceites del Aljarafe S.L." está buscando una propuesta técnica de implantación que cubra los 3 siguientes bloques.

## Cálculo de TCO con una estimación de 3 años.
Coste de licencias/suscripción.
Pese a que la edición Community de Odoo es gratuita, si se quiere hacer uso de la edición Enterprise, existirá un cargo, dependiendo del número de usuarios y módulos instalados. 
En nuestro caso, el plan que elegiremos será el Plan Personalizado. Existen dos tipos entre los que se da a elegir dentro de Odoo. El primero de ellos es el Plan Estándar, que es más barato, pero que obliga a utilizar el hosting de Odoo Online. 
Hemos descartado esta opción, debido a que queremos otro servicio de hosting. Por ello, nos hemos decantado por el Plan Personalizado, que tiene un coste total de 560€ al mes, para un tamaño total de 25 empleados. Siendo que vamos a calcularlo en un lapso de 3 años, hemos preferido contratar de forma anual, ya que se hace un pequeño descuento, dando un total de 447.5€ mensuales. Para los tres años, esto dará un total de 16110€.

Coste operativo (Hosting en Google Cloud, AWS, Huawei Cloud o similar).
Tras observar los precios de los direfentes Hosting, el más adecuado a la empresa con el número de empleado es el Google Cloud. Tiene un coste de 300$ al año, por lo que de aquí a tres años sería un total de 900$.

Para ello, el total de gasto es de 17010€. 


## Diseño de Seguridad RBAC
Bloque B
Administrador: Acceso total.
Tenemos 2 administradores con acceso total. Puede realizar operaciones como crear, leer o consultar, actualizar y borrar o eliminar. Lleva a cabo las funciones que un usuario necesita para crear y gestionar datos.
Comercial: Solo ve sus clientes y presupuestos (Record Rules).
8 comerciantes, así pueden poner puestas en común de los distintos presupuestos que van saliendo con la mercancía  a la vez que los clientes ofrecen ciertos productos.
Operario de Almacén: Solo ve stock y albaranes de entrada/salida.
12 en almacén. Podrán apoyarse en la reposiciones de los productos que se queden sin el stock y observar la entrada y salida de los productos. Si ven algún error, lo comunican a los administradores. 
Contable: Puede mirar facturas pero no puede modificar el stock.
3 contables que pueden llevar a cabo los roles de elaborar presupuestos, registrar pagos e ingresos, pagar facturas y controlar cobros, preparar declaraciones fiscales y crear informes contables y financieros.


Documentación de Explotación
Bloque C
Manual de Despliegue 
Hemos creado un documento docker-compose.yml para la gestión. En caso de pérdida de información, usaremos el comando pg_dump -U postgres -d db12 > backup.sql, que creará una copia de seguridad. Para recuperar esta copia, se utilizará psql -U postgres -d db12 < backup.sql. 

## Bibliografía
[1] RGB Consulting, "¿Cuánto vale Odoo?," RGB Consulting Blog, 2024. [En línea]. Disponible en: https://www.rgbconsulting.com/blog/blog-6/cuanto-vale-odoo-64. [Accedido: 22-may-2024]. 

[2] Amazon Web Services, "Precios de productos y servicios de AWS," AWS, 2024. [En línea]. Disponible en: https://aws.amazon.com/es/pricing/. [Accedido: 22-may-2024]. 

[3] Huawei Cloud, "Pricing Calculator: Elastic Cloud Server (ECS)," Huawei Cloud, 2024. [En línea]. Disponible en: https://www.huaweicloud.com/eu/pricing/calculator.html#/ecs. [Accedido: 22-may-2024]. 

