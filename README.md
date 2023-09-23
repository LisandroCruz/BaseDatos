# ServiTech
# Manual de Usuario
Instrucciones básicas del proyecto

Al momento de iniciar el programa visualizaremos lo siguiente:

Pantalla de Inicio de Sesión: podemos ingresar nuestro correo electrónico y contraseña si ya tenemos una cuenta creada. La aplicación tiene validaciones cuando un usuario intenta iniciar sesión. Si la contraseña o el correo electrónico son incorrectos, aparecerá una advertencia que indicará que uno de los campos tiene valores incorrectos. Suponiendo que no tienes una cuenta, pasa al siguiente paso.

Pantalla de Registro: En esta pantalla podemos crear una nueva cuenta. Dentro de esta pantalla tenemos diferentes campos:

Nombre
Apellido
Correo electrónico
Contraseña
Todos los campos son obligatorios para crear una nueva cuenta, la aplicación valida si el correo electrónico que estás ingresando ya está siendo utilizado por otro usuario. Una vez que hayas creado tu cuenta y hayas iniciado sesión, podemos pasar al siguiente paso.

Página del Panel de Control: Al inicio de la aplicación, una vez que hayas iniciado sesión, en la parte superior de la aplicación verás tu nombre, el que utilizaste para registrar tu cuenta. En el lado derecho verás el logotipo y el nombre de la empresa. La aplicación está dividida en 3 partes:

Datos

Operaciones

Inventario

Datos: Esta sección tiene los campos para crear un nuevo producto en el inventario, que incluye los siguientes campos:

Nombre del producto
Cantidad del producto (esto se establece en 0 de forma predeterminada)
Precio del producto
Esta parte también contiene 2 botones adicionales, Insertar y Continuar, que se mostrarán una vez que se seleccione una operación para incluir un nuevo producto en el inventario o extraer uno.

Operaciones: Esta parte de la aplicación contiene todos los botones que se utilizarán para realizar operaciones, que son los siguientes:

Extraer Esto mostrará un cuadro modal para que el usuario ingrese un ID de producto para realizar una extracción del inventario. Una vez que se encuentra un producto, mostrará un cuadro modal para que el usuario ingrese la información del usuario para crear la factura, todos los formularios y campos tienen validaciones.
Insertar Este botón abrirá un formulario para que el usuario ingrese un ID de producto. Si se encuentra un producto, todos los demás botones se deshabilitarán, dejando solo el campo para actualizar la nueva cantidad.
Buscar El botón de búsqueda abrirá un cuadro modal para que el usuario busque un producto por ID.
Nuevo producto El botón de agregar nuevo producto insertará en la base de datos una vez que se completen todos los campos en la sección de Datos.
Informe El botón de informe activará una función que buscará en la base de datos todos los productos que pertenecen al usuario actualmente registrado y creará un PDF con todos los productos.
Eliminar El botón de eliminar mostrará un cuadro modal para que el usuario busque si el producto está en la base de datos y solicitará confirmación para eliminar permanentemente el producto de la base de datos.
Cerrar sesión El botón cerrará la sesión actual.
Inventario: Esta sección contiene una tabla con 6 columnas

ID del producto Contiene el ID del producto.
Nombre del producto Contiene el nombre del producto.
Existencia actual Contiene la cantidad actual del producto.
Precio unitario del producto Contiene el precio individual del producto.
Cantidad total Contiene la cantidad total para el precio actual.
Última modificación Contiene la última fecha de actualización del producto.
En la parte inferior de la aplicación, verás el monto total en $ de todos los productos.
