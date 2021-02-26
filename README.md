# Trabajo1
Trabajo1 comunicación escrita
Proyecto
La tarea principal de este proyecto es resolver sudokus. El usuario introduce valores en un sudoku hecho en una interfaz gráfica y regresa la solución o en el caso de que no tenga solución, regresa “no tiene solución”. Cuando el usuario ingresa más de 17 valores la respuesta se vuelve única.
Este proyecto fue asignado para demostrar y desarrollar habilidades en las estructuras de datos básicas como arreglos y listas. Así como, el uso de fuerza bruta para resolver tareas.

# Manual del desarrollador
El proyecto se divide en dos partes principales: solucionador e interfaz gráfica. 

Solucionador
La primera parte es donde está el código que da respuesta al sudoku. Se basa en una matriz de 9 por 9 que recorre los renglones de arriba hacia abajo con el uso de arreglos, if, for y while. 
Con base en los datos ingresados por el usuario el solucionador empieza con la primera casilla disponible y le asigna un valor entre el 1 y el 9, empezando por el 1. Se checa que el renglón cumpla con las reglas del sudoku y luego, que la columna también las cumpla. 
Se avanza a la siguiente casilla y si no puede avanzar se regresa para intentar con otro valor. Progresa de esta forma hasta lograr asignar un valor a la última casilla siguiendo las reglas del juega y regresa la solución.
El solucionador empieza con las funciones básicas de la clase y termina con la función respuesta() que es llamada para obtener la solución del sudoku. La función valido() es para que los objetos introducidos en las casillas sean enteros y estén en el rango válido. La función renglón() checa que en el arreglo renglón no tenga ningún valor repetido. La función columna() checa que la columna no tenga ningún valor repetido. Sigue la función cuadrante() que consta de 9 matrices de 3x3 en las que se divide la matriz general y checa que en el cuadrante no haya números repetidos.
Estas funciones son parte de la función respuesta(), la cual está conectada a la interfaz gráfica y da solución al sudoku planteado por el usuario.

Interfaz gráfica 
Esta parte es muy básica e intuitiva. El propósito de la interfaz gráfica es facilitar al usuario ingresar los valores a la matriz y facilitar la lectura de la respuesta al sudoku.
Se tiene casillas que están asignadas a cada espacio de la matriz de arreglos. Los valores ingresados en esas casillas se acomodan en la matriz. Además, se cuenta con el botón de limpiar para limpiar el sudoku y con el botón respuesta que llama a la función respuesta() y da una solución. 

# Manual de usuario
El usuario al correr el programa obtiene la interfaz gráfica. El uso del proyecto es muy sencillo. Se ingresan números del 1 al 9 en las casillas dándole clic a cada casilla, sin repetir números en los renglones, en las columnas o en los cuadrantes, o se regresa “no tiene solución”. 
Cuando el interfaz tenga ya todos los valores deseados se pulsa el botón respuesta y la interfaz va a cambiar al sudoku resuelto para los valores ingresados. La respuesta es única cuando el usuario ingresa más de 17 valores. En caso contrario, hay más respuestas posibles y el proyecto va a regresar la primera que encuentre.
El botón limpiar pone en blanco todas las casillas de la interfaz gráfica, esto sirve para cuando ya se dio una respuesta y se quieren ingresar otros valores. Además, sirve para cuando se quieren eliminar TODOS los valores ingresados.

# Conclusión
Usen este proyecto de la manera que les sea más útil, pueden tomar las partes o las funciones que les sirvan o modifíquenlo para adaptarse a sus necesidades y gustos.
