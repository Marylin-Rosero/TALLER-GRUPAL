# TALLER-GRUPAL
TALLER GRUPAL
![image](https://github.com/Marylin-Rosero/TALLER-GRUPAL/assets/169502533/d10b685b-6fdc-4ab8-86e0-bf67a0b265aa)
![image](https://github.com/Marylin-Rosero/TALLER-GRUPAL/assets/169502533/a29c4f9a-a790-4294-8033-0589af648af1)
![image](https://github.com/Marylin-Rosero/TALLER-GRUPAL/assets/169502533/a9dedb93-3ddb-4292-8092-3989229904e4)
![image](https://github.com/Marylin-Rosero/TALLER-GRUPAL/assets/169502533/b04197d9-6ff6-4527-a7ed-28014f4d8e7d)
El código crea una aplicación de escritorio en Java que muestra información sobre los constructores de Fórmula 1 de un año específico seleccionado por el usuario. A continuación se detalla lo que hace el código y qué presenta:

Lo que Hace el Código
Conexión a la Base de Datos:

Se conecta a una base de datos PostgreSQL que contiene información sobre carreras de Fórmula 1.
Creación de la Interfaz Gráfica:

Crea una ventana (JFrame) con un título descriptivo.
Añade un menú desplegable (JComboBox) para que el usuario pueda seleccionar un año.
Añade una tabla (JTable) que muestra información sobre los constructores de Fórmula 1 para el año seleccionado.
Usa un DefaultTableCellRenderer para centrar el contenido de las celdas de la tabla.
Poblar el Menú Desplegable:

Llena el JComboBox con años disponibles obtenidos de la base de datos.
Actualizar la Tabla en Segundo Plano:

Cuando el usuario selecciona un año en el JComboBox, se ejecuta una consulta en segundo plano usando SwingWorker para obtener los datos de los constructores de ese año.
La consulta SQL obtiene el nombre del constructor, el número de victorias, los puntos totales y la posición en el ranking.
Los datos obtenidos se utilizan para actualizar el modelo de la tabla, que a su vez actualiza la vista en la interfaz gráfica.
Qué Presenta el Código
Interfaz de Usuario:

Una ventana (JFrame) titulada "Tabla de Constructores por Año".
Menú Desplegable:

Un JComboBox en la parte superior de la ventana, que permite al usuario seleccionar un año.
Tabla de Datos:

Una JTable en el centro de la ventana que muestra la siguiente información sobre los constructores de Fórmula 1 para el año seleccionado:
Constructors: El nombre del constructor.
Wins: El número de victorias.
Total Points: Los puntos totales acumulados.
Rank: La posición en el ranking basado en los puntos totales.
La tabla se actualiza dinámicamente en función del año seleccionado por el usuario, proporcionando una vista interactiva y actualizada de los datos de los constructores.
