# COMANDOS

<h2>Comandos BASICOS de MySql</h2>

1.  Comando para conectar a la base de datos:

        mysql -u usuario -p

2.  Comando para mostrar todas las bases de datos:

        SHOW DATABASES;

3.  Comando para seleccionar una base de datos específica:

        USE nombre_de_la_base_de_datos;

4.  Mostrar todas las tablas en una base de datos:

        SHOW TABLES;

5.  Mostrar la estructura de una tabla:

        DESCRIBE nombre_de_la_tabla;

6.  Realizar una consulta SELECT:

        SELECT columna1, columna2 FROM nombre_de_la_tabla;

7.  Insertar datos en una tabla:

        INSERT INTO nombre_de_la_tabla (columna1, columna2) VALUES (valor1, valor2);

8.  Actualizar datos en una tabla:

        UPDATE nombre_de_la_tabla SET columna1 = valor1 WHERE condicion;

9.  Eliminar datos de una tabla:

        DELETE FROM nombre_de_la_tabla WHERE condicion;

<h2>Comandos de MySql para realizar CONSULTAS DESDE LA TERMINAL</h2>

1.  Filtrar resultados con WHERE:

        SELECT columna1, columna2 FROM nombre_de_la_tabla WHERE condicion;

    Este comando permite agregar una condición para filtrar los resultados de una consulta.<br>
    Puedes utilizar operadores como "=", "<", ">", "<=", ">=", "!=" para comparar valores.

2.  Ordenar resultados con ORDER BY:

        SELECT columna1, columna2 FROM nombre_de_la_tabla ORDER BY columna1 ASC|DESC;

    Permite ordenar los resultados de una consulta en función de una o varias columnas,
    <br>en orden ascendente (ASC) o descendente (DESC).

3.  Limitar resultados con LIMIT:

        SELECT columna1, columna2 FROM nombre_de_la_tabla LIMIT cantidad;

    Limita el número de filas que se devuelven en una consulta. Puedes especificar<br>
    la cantidad de filas que deseas mostrar.

4.  Realizar operaciones matemáticas:

        SELECT columna1, columna2, columna1 + columna2 AS suma FROM nombre_de_la_tabla;

    Puedes realizar operaciones matemáticas en una consulta, como suma, resta, multiplicación<br>
    y división, utilizando los operadores correspondientes (+, -, \*, /).

5.  Utilizar funciones de agregación:

        SELECT COUNT(columna1) AS cantidad FROM nombre_de_la_tabla;

    Las funciones de agregación, como COUNT, SUM, AVG, MIN y MAX, permiten realizar cálculos<br>
    sobre un conjunto de valores en una columna.

6.  Unir tablas con JOIN:

        SELECT columna1, columna2 FROM tabla1 JOIN tabla2 ON tabla1.columna = tabla2.columna;

    JOIN permite combinar filas de dos o más tablas en función de una condición de unión.

7.  Realizar consultas condicionales con CASE:

        SELECT columna1, CASE WHEN columna2 = 'valor' THEN 'Condición cumplida' ELSE 'Condición no cumplida' END AS resultado FROM nombre_de_la_tabla;

    CASE permite realizar consultas condicionales, donde puedes especificar diferentes resultados<br>
    según una condición.

/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/
/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/_/  

# Aqui hay como una breve explicacion de cómo hacer consultas en MySQL y algunos ejemplos:

<h3>1. Consulta básica SELECT:</h3>

<p>La sintaxis básica para realizar una consulta SELECT es la siguiente:</p>

         SELECT columna1, columna2 FROM nombre_de_la_tabla;

<h5>Ejemplo:</h5>
<p>Supongamos que tenemos una tabla llamada "clientes" con las columnas "id", "nombre" y "email". Para obtener todos los<br>
 registros de la tabla, ejecutaríamos la siguiente consulta:</p>

        SELECT * FROM clientes;


<h3>2.  Filtrar resultados con WHERE:</h3>
<p>Puedes agregar una cláusula WHERE para filtrar los resultados según una condición.</p>
<h5>Ejemplo:</h5>

         SELECT * FROM clientes WHERE nombre = 'Juan';

<p>Esta consulta devolverá todos los registros de la tabla "clientes" donde el nombre sea igual a 'Juan'.</p>

<h3>3. Ordenar resultados con ORDER BY:
   <p>Puedes ordenar los resultados de una consulta utilizando ORDER BY.</p>
<h5>Ejemplo:</h5>

       SELECT \* FROM clientes ORDER BY nombre ASC;

   <p>Esta consulta ordenará los registros de la tabla "clientes" en orden ascendente según la columna "nombre".</p>

<h3>4. Limitar resultados con LIMIT:</h3>
   <p>Puedes limitar el número de filas que se devuelven en una consulta utilizando LIMIT.</p>
   <h5>Ejemplo:</h5>

        SELECT \* FROM clientes LIMIT 10;

   <p>Esta consulta devolverá los primeros 10 registros de la tabla "clientes".</p>


<h3>5. Realizar operaciones matemáticas:</h3>
   Puedes realizar operaciones matemáticas en una consulta. 

   <h5>Ejemplo:</h5>

        SELECT precio, cantidad, precio \* cantidad AS total FROM productos;

   <p>Esta consulta multiplicará los valores de las columnas "precio" y "cantidad" y mostrará el resultado en una columna llamada "total".</p>

