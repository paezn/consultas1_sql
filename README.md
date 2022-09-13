# consultas1_sql

# EJERCICIOS CONSULTAS SQL

## Tabla usuario

![tabla usuario](img/tabla_usuario.png "Tabla usuario")

1. Para visualizar toda la información que contiene la tabla `usuario` se puede incluir con la instrucción SELECT el caracter '*' o cada uno de los campos de la tabla 

`select * from usuario` 

![Consulta1](img/consulta1.png "Consulta1")

2. Visualizar solamente la identificación del usuario.

`select Identificacion from usuario`

![Consulta2](img/consulta2.png "Consulta2")

3. Si se desea obtener los registros cuya identificación sean mayores o iguales a 150, se debe utilizar la clausula WHERE que especifica las condiciones que deben reunir los registros que se van a seleccionar.

`SELECT * FROM usuario WHERE Identificación>='150'`

![Consulta3](img/consulta3.png "Consulta3")

4. Si se desea obtener los registros cuyo sus apellidos sean Vanegas o Cetina, se debe utilizar el operador IN que especifica los registros que se quieren visualizar de una tabla.

`SELECT apellidos FROM usuario WHERE apellidos IN ('Vanegas','Cetina')`

![Consulta4](img/consulta4.png "Consulta4")

O se puede utilizar el operador OR.

`SELECT apellidos FROM usuario WHERE apellidos='Vanegas' OR apellidos='Cetina'`

![Consulta4](img/consulta4_2.png "Consulta4")

5. Si se desea obtener los registros cuya identificación sea menor de '110' y la ciudad sea 'Cali', se debe utilizar el operador AND.

`SELECT * FROM usuario WHERE Identificación<'110' AND ciudad_nac='Cali'`

![Consulta5](img/consulta5.png "Consulta5")

6. Si se desea obtener los registros cuyos nombres empiecen por la letra 'A', se debe utilizar el operador LIKE que utiliza los patrones '%' (todos) y '_' (caracter).

`SELECT * FROM usuario WHERE nombre LIKE 'A%'`

![Consulta6](img/consulta6.png "Consulta6")

7. Si desea obtener los registros cuyos nombres contengan la letra 'a'.

`SELECT * FROM usuario WHERE nombre LIKE '%a%'`

![Consult7](img/consulta7.png "Consulta7")
