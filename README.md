# Español

# ServiTech

# Manual de Usuario
Instrucciones básicas del proyecto

Al momento de iniciar el programa visualizaremos lo siguiente:

# Inicio de sesión

Pantalla de Inicio de Sesión: La pantalla de inicio de sesión mostrara dos campos a rellenar los cuales son: Usuario y Contraseña, el usuario y contraseña han sido predifinidos por mi para que el proceso sea más rápido.
Usuario: Lisandro
Contraseña: 12345
Luego de haber rellenado los campos con los datos previos solamente hace falta hacer click izquierdo sobre el botón de "ingresar"
Una vez ingresado, en pantalla podremos observar el programa ejecutandose y mostrara lo siguiente:

# CRUD del programa

Código

Nombre del producto

Precio unitario

Cantidad de Unidades

Fecha de ingreso



Los datos mencionados anteriormente son campos a rellenar por quien este utilizando el programa.

Inferior a estos podremos visualizar el apartado de opciones que cuenta con 7 botónes, en órden de izquierda a derecha son:

Agregar

Modificar

eliminar

salir

reporte

buscar

refrescar

# Como funcionan los botónes del programa
Si queremos agregar un prodocuto deberemos de rellenar todos los campos solicitados y luego de rellenar los campos simplemente hacemos click izquierdo sobre el botón de agregar.

# Agregar
Para modificar un producto debemos de ingresar el código de un producto agregado previamente y en todos los demás campos tenemos que colocar datos nuevos.

# Eliminar

Para eliminar simplemente tenemos que colocar en el campo de código el código de un producto previamente creado y dar click sobre el botón de eliminar y el producto será eliminado

# Salir

Para salir del programa simplemente debemos de dar click en el botón de salir

# Reporte

Para generar un reporte es tan simple como dar click en el botón de generar reporte y automáticamente se generara un reporte con todos los productos creados por el usuario

# Buscar

Para buscar un producto debemos de rellenar ya sea el campo de código o de nombre del producto y dar click en el botón de buscar

# Refrescar

Y por último el botón de refrescar tiene la funcionalidad de regresar al estado base la tabla, esto quiere decir, que si realizamos una búsqueda en la tabla de productos que esta situada en la parte inferior del programa nos apareceran solo los productos que coincidan con el código o nombre colocados en los campos y al hace click en el botón refrescar la tabla nos mostrara nuevamente todos los productos y los campos de código y nombre serán vacíados.

# Inglés

# ServiTech

# User Manual

Basic Project Instructions

When you start the program, you will see the following:

# Login

Login Screen: The login screen will display two fields to fill in, which are: User and Password. The user and password have been predefined by me to make the process faster.
User: Lisandro
Password: 12345
After filling in the fields with the provided data, simply click the "Login" button.
Once logged in, the program will run on the screen and display the following:

# Program CRUD

Code

Product Name

Unit Price

Quantity of Units

Date of Entry

The mentioned data fields above need to be filled in by the user of the program.

Below these fields, you will see the options section with 7 buttons, from left to right:

Add

Edit

Delete

Exit

Report

Search

Refresh

# How the Program Buttons Work
If you want to add a product, you need to fill in all the required fields, and after filling in the fields, simply click the "Add" button.

# Add
To edit a product, you must enter the code of a previously added product, and in all other fields, you must enter new data.

# Delete

To delete, simply enter the code of a previously created product in the code field and click the "Delete" button, and the product will be deleted.

# Exit

To exit the program, simply click the "Exit" button.

# Report

To generate a report, simply click the "Generate Report" button, and a report with all the products created by the user will be automatically generated.

# Search

To search for a product, fill in either the code field or the product name field and click the "Search" button.

# Refresh

Finally, the refresh button has the functionality of returning the table to its base state. This means that if you perform a search in the product table located at the bottom of the program, only the products that match the code or name entered in the fields will appear. Clicking the refresh button will display all the products again, and the code and name fields will be cleared.


# Imágenes del manual de usuario

![image](https://github.com/LisandroCruz/BaseDatos/assets/145726150/845a008d-74a3-46d4-93af-52c4f7e298df)

![image](https://github.com/LisandroCruz/BaseDatos/assets/145726150/f79f8347-6f69-4070-a5f2-6ea78da4a448)

![image](https://github.com/LisandroCruz/BaseDatos/assets/145726150/275adfd8-926d-42d8-914f-27523ad7a176)



# Manual técnico

Introducción
La aplicación Java "bdnegocio" es un programa sencillo para gestionar datos de productos en una base de datos. Este manual técnico proporciona una visión general de la estructura del código, su funcionalidad y cómo interactúa con la base de datos.

Estructura del Código
El código de la aplicación "bdnegocio" está organizado en las siguientes secciones:

Importaciones: Esta sección incluye declaraciones de importación para varias bibliotecas y clases de Java que se utilizan en la aplicación. Estas importaciones incluyen clases para trabajar con componentes Swing, JDBC para la conectividad con la base de datos y JasperReports para generar informes.

Declaración de Clase: La clase principal de la aplicación se llama "bdnegocio" y extiende javax.swing.JFrame. Esta clase representa la ventana principal de la aplicación.

Variables de Instancia: Se declaran varias variables de instancia a nivel de clase, incluyendo objetos para la conexión a la base de datos (conet), un modelo de tabla (modelo) para gestionar la tabla de datos de productos y otras variables para la interacción con la base de datos.

Constructor: La clase "bdnegocio" tiene un constructor que inicializa los componentes de la interfaz de usuario gráfica (GUI), establece sus propiedades y establece una conexión con la base de datos.

Inicialización de Componentes de GUI: Los componentes de la GUI, incluyendo etiquetas, campos de texto, botones y tablas, se inicializan y configuran en el método initComponents. Este método configura el diseño y la apariencia de la ventana de la aplicación.

Oyentes de Acción: Se definen métodos de oyentes de acción para varios botones en la GUI. Estos métodos manejan las interacciones del usuario, como agregar, editar, eliminar, generar informes, buscar y actualizar datos de productos.

Método Principal: El método principal es el punto de entrada de la aplicación. Establece el aspecto de la aplicación y crea una instancia de la clase "bdnegocio" para iniciar la aplicación.

Consulta de Datos: El método "consultar" recupera datos de la base de datos y llena la tabla de productos con los resultados. Utiliza consultas SQL para obtener información de productos de la base de datos y actualizar el modelo de tabla.

1. Agregar Productos

Proceso:

1. El usuario ingresa información del producto (código, nombre, precio unitario, cantidad y fecha de ingreso) en los campos de texto respectivos en la GUI.
2. El usuario hace clic en el botón "Agregar".

Explicación del Código:

- En el método "jButton1ActionPerformed", se recoge la entrada del usuario de los campos de texto.
- Se prepara una declaración SQL "INSERT" para agregar los datos del producto a la base de datos.
- Se llama al método "executeUpdate" para ejecutar la declaración SQL y agregar el producto a la base de datos.
- Después de la inserción exitosa, se llama al método "consultar" para actualizar la tabla de productos con los nuevos datos.

2. Modificar Productos

Proceso:

1. El usuario ingresa el código del producto (para identificar el producto a modificar) y actualiza el nombre, el precio unitario, la cantidad y la fecha de ingreso en los campos de texto respectivos en la GUI.
2. El usuario hace clic en el botón "Modificar".

Explicación del Código:

- En el método "jButton2ActionPerformed", se recoge la entrada del usuario, incluyendo el código del producto para su identificación.
- Se prepara una declaración SQL "UPDATE" para modificar los datos del producto en la base de datos según el código del producto.
- Se llama al método "executeUpdate" para ejecutar la declaración SQL y actualizar el producto en la base de datos.
- Después de la modificación exitosa, se llama al método "consultar" para actualizar la tabla de productos.

3. Eliminar Productos

Proceso:

1. El usuario ingresa el código del producto (para identificar el producto a eliminar) en el campo de texto de código en la GUI.
2. El usuario hace clic en el botón "Eliminar".

Explicación del Código:

- En el método "jButton3ActionPerformed", se recoge la entrada del usuario (código del producto) desde la interfaz.
- Se prepara una declaración SQL "DELETE" para eliminar el producto de la base de datos según el código del producto.
- Se llama al método "executeUpdate" para ejecutar la declaración SQL y eliminar el producto de la base de datos.
- Después de la eliminación exitosa, se llama al método "consultar" para actualizar la tabla de productos.

4. Generar Informes

Proceso:

1. El usuario hace clic en el botón "reporte" en la GUI.

Explicación del Código:

- En el método "jButton5ActionPerformed", se genera un informe de JasperReports.
- Se carga la plantilla del informe desde una ruta de archivo específica.
- Se establece la conexión con la base de datos.
- Se obtienen datos de la base de datos mediante consultas SQL.
- Los datos obtenidos se llenan en la plantilla del informe.
- El informe se muestra en un visor de Jasper.

5. Buscar Productos

Proceso:

1. El usuario ingresa el código del producto o el nombre del producto (o ambos) en los campos de texto respectivos en la GUI.
2. El usuario hace clic en el botón "buscar" en la GUI.

Explicación del Código:

- En el método "jButton6ActionPerformed", se construye una consulta SQL dinámica en función de la entrada del usuario (código y nombre).
- Se ejecuta la consulta SQL para recuperar productos coincidentes de la base de datos.
- La tabla de productos se actualiza con los resultados de la búsqueda.

6. Actualizar la Tabla de Productos

Proceso:

1. El usuario hace clic en el botón "refrescar" en la GUI.

Explicación del Código:

- En el método "jButton7ActionPerformed", se llama al método "consultar" para recuperar todos los datos de productos de la base de datos y actualizar la tabla de productos.

7. Salir de la Aplicación

Proceso:

1. El usuario hace clic en el botón "salir" en la GUI.

Explicación del Código:

- En el método "jButton4ActionPerformed", se utiliza la declaración "System.exit(0)" para cerrar la aplicación.


# Technical Manual 

Introduction
The "bdnegocio" Java application is a simple program for managing product data in a database. This technical manual provides an overview of the code structure, its functionality, and how it interacts with the database.

Code Structure
The code for the "bdnegocio" application is organized into the following sections:

Imports: This section includes import statements for various Java libraries and classes that are used in the application. These imports include classes for working with Swing components, JDBC for database connectivity, and JasperReports for generating reports.

Class Declaration: The main class for the application is named bdnegocio, which extends javax.swing.JFrame. This class represents the main application window.

Instance Variables: Several instance variables are declared at the class level, including objects for database connection (conet), a table model (modelo) for managing the product data table, and other variables for database interaction.

Constructor: The bdnegocio class has a constructor that initializes the application's graphical user interface (GUI) components, sets their properties, and establishes a database connection.

Initialization of GUI Components: The GUI components, including labels, text fields, buttons, and tables, are initialized and configured in the initComponents method. This method sets up the layout and appearance of the application window.

Action Listeners: Action listener methods are defined for various buttons in the GUI. These methods handle user interactions such as adding, editing, deleting, generating reports, searching, and refreshing the product data.

Main Method: The main method is the entry point of the application. It sets the look and feel of the application and creates an instance of the bdnegocio class to start the application.

Consulting Data: The consultar method retrieves data from the database and populates the product table with the results. It uses SQL queries to fetch product information from the database and update the table model.

1. Adding Products
   
Process:

User enters product information (code, name, unit price, quantity, and date of entry) into the respective text fields in the GUI.
User clicks the "Agregar" (Add) button.
Code Explanation:

In the jButton1ActionPerformed method, the user input from the text fields is retrieved.
A SQL INSERT statement is prepared to add the product data to the database.
The executeUpdate method is called to execute the SQL statement and add the product to the database.
After successful insertion, the consultar method is called to update the product table with the new data.

2. Modifying Products

Process:

User enters the product's code (to identify the product to be modified) and updates the name, unit price, quantity, and date of entry in the respective text fields in the GUI.
User clicks the "Modificar" (Edit) button.
Code Explanation:

In the jButton2ActionPerformed method, the user input is retrieved, including the product code for identification.
A SQL UPDATE statement is prepared to modify the product data in the database based on the product code.
The executeUpdate method is called to execute the SQL statement and update the product in the database.
After successful modification, the consultar method is called to update the product table.

3. Deleting Products
   
Process:

User enters the product's code (to identify the product to be deleted) into the code text field in the GUI.
User clicks the "Eliminar" (Delete) button.
Code Explanation:

In the jButton3ActionPerformed method, the user input (product code) is retrieved.
A SQL DELETE statement is prepared to remove the product from the database based on the product code.
The executeUpdate method is called to execute the SQL statement and delete the product from the database.
After successful deletion, the consultar method is called to update the product table.

4. Generating Reports
   
Process:

User clicks the "reporte" (Report) button in the GUI.

Code Explanation:

In the jButton5ActionPerformed method, a JasperReports report is generated.

The report template is loaded from a specific file path.

The database connection is established.

Data from the database is fetched using SQL queries.

The fetched data is filled into the report template.

The report is displayed in a JasperViewer.

5. Searching Products
   
Process:

User enters either the product code or product name (or both) into the respective text fields in the GUI.
User clicks the "buscar" (Search) button.
Code Explanation:

In the jButton6ActionPerformed method, a dynamic SQL query is constructed based on the user's input (code and name).
The SQL query is executed to retrieve matching products from the database.
The product table is updated with the search results.
6. Refreshing the Product Table
Process:

User clicks the "refrescar" (Refresh) button in the GUI.
Code Explanation:

In the jButton7ActionPerformed method, the consultar method is called to retrieve all product data from the database and refresh the product table.
7. Exiting the Application
Process:

User clicks the "salir" (Exit) button in the GUI.
Code Explanation:

In the jButton4ActionPerformed method, the System.exit(0) statement is used to terminate the application.

# Enlaces de apoyo

CRUD:

https://www.youtube.com/watch?v=6_ncKPDvKEg

Reportes con Jasper:

https://www.youtube.com/watch?v=KSdHTGhHrIU&t=1194s
