# Programas en c++ de Mejia Jose
> Aquí encontrarás el instructivo de como manejar los programas desarrollados en este directorio.
> Todos los programas desarrollados a continuación se encuentran en lenguaje c++.
## Informacion del autor
  Creado por: José Eduardo Mejía Micolta.
  
  Correo institucional: jose.mejia.micolta@utelvt.edu.ec
  
  Correo Personal: mejiamicoltalol@gmail.com
  
  Video de introducción sobre informática: https://youtu.be/1aOKP2YPzlk
  
 ## Programas
  ### Programa para comparar dos números
  * #### Descripción del problema que soluciona
  El programa permite comparar dos numeros ingresados de manera manual por el usuario, y determinar cuando estos numeros son iguales o cuando uno de ellos es mayor al otro. 
  * #### Funcionalidad
  En este programa vamos a usar variable de tipo decimal (`float`).
  
  El programa nos permite ingresar las dos cantidades que deseamos comparar, las cuales van a estar almacenadas en `jm_num1` y `jm_num2` respectivamente.
  
  Una vez ingresadas las variables, utilizaremos la función `if` para poder hacer una comparación lógica entre las cantidades ingresadas.
  * #### Salidas
  Una vez realizado el proceso lógico, se pueden imprimir un total de tres posibilidades:
  
  * La primera:
  `Ambas cantidades son iguales` (en caso de que los numeros ingresados sean iguales).
  * La segunda:
  `El número jm_num1 es mayor que jm_num2` (en caso de que el primer numero ingresado sea mayor al segundo).
  * La tercera:
  `El numero jm_num2 es mayor que jm_1` (en caso de que el segundo numero ingresado sea mayor al primero).
  > Imagen de referencia:
  > 
  > ![Compara](https://github.com/josemm0505/Practica1/blob/main/Codigo_Compara.jpg)
 
  ### Programa para sumar varios números
  * #### Descripción del problema que soluciona
  El programa permite sumar la cantidad de numeros que el usuario desee, ingresandolos todos de manera manual.
  * #### Funcionalidad
  En este programa vamos a usar dos tipos de datos; los enteros (`int`), y los decimales (`float`).
  
  Vamos a requerir, de igual manera, el uso de un contador (`jm_i` que va a estar declarado como un entero) y el uso de un acumulador (`jm_s` que va a estar declarado como decimal).
  
  El contador va a ir incrementando de uno en uno, en función del numero que ingrese el usuario (`jm_n`). 
  
  El acumulador va a ir almacenando la suma de las cantidades que ingrese el usuario (`jm_x`).
  
  Para complementar este proceso, vamos a usar una estructura repetitiva `do-while`, que servirá para que el proceso anteiormente descrito, se repita mientras se cumpla una condición (`jm_i<jm_n`).
  
  * #### Salidas
  Una vez realizado todo el proceso, el programa va a imprimir el valor del contador (`jm_n`) y el valor del acumulador (`jm_s`).
  > Imagen de referencia:
  > 
  > ![SumaN](https://github.com/josemm0505/Practica1/blob/main/Codigo_SumaN.jpg)

  ### Programa para para calcular el punto de venta
  * #### Descripción del problema que soluciona
  El programa permite ingresar el valor de las comprar que el usuario desee, calcula el valor del IVA  de la compra, aplica un descuento a elección del usuario, para finalmente, mostrar el valor bruto de la compra, el valor del IVA, el valor del descuento, y el precio final a pagar.
  * #### Funcionalidad
  Para este programa, vamos a usar variables de tipo entero (`int`) y variables de tipo decimal (`float`).
  
  De igual manera, vamos a requerir del uso de un contador (`jm_c`) y el uso de un acumulador (`jm_s`)
  
  El contador va a ir incrementando de uno en uno, en función del número de compras que el usuario desee ingresar (`jm_n`).
  
  El acumulador va a ir almacenando la suma de los valores de cada unas de las compras que ingrese el usuario (`jm_x`).
  
  Para complementar este proceso, vamos a utilizar una estructura repetitiva `do-while`, que servirá para que el proceso anteriormente descrito, se repita mientras se cumpla una condición (`jm_c<jm_n`).
  
  Una vez que hemos ingresado, sumado y almencenado el valor bruto de las compras (`jm_s`), tenemos que aplicarle un descuento. Para ello, le pedimos al usuario que ingrese el descuento que desee aplicar (`jm_d`).
  
  Posterior a esto, se realizan los siguientes procesos:
  > `jm_t=(jm_s*jm_d)/100;`(la variable `jm_t` va a almacenar el resultado del descuento que se le aplique a la compra).
  > 
  > `jm_t1=jm_s-jm_t;` (la variable `jm_t1` va a almacenar el resultado de la diferencia entre el valor acumulado de las compras, y el valor resultante del descuento).
  > 
  > `jm_iv=jm_t1*0.12` (la variable `jm_iv` va a almacenar el calculo del IVA de la variable anterior `jm_t1`).
  > 
  > `jm_f=(jm_s-jm_t)+jm_iv;` (la variable `jm_f` va a almacenar el resultado final, en el cual se va a aplicar el descuento, y añadir el IVA).
  * #### Salidas
  Una vez que se realiza todo este proceso, el programa nos va a imprimir los siguientes valores:
  > `jm_s` (variable que representa el valor bruto de las compras).
  > 
  > `jm_t` (variable que representa el valor de la compra, aplicandole el descuento).
  > 
  > `jm_iv` (variable que representa el valor de la compra, añadiendole el IVA).
  > 
  > `jm_f` (variable que representa el valor final).
 
  > Imagen de referencia:
  > 
  > ![PuntoVenta](https://github.com/josemm0505/Practica1/blob/main/Codigo_PuntoVenta.jpg)
  ### Programa para saber la edad de una persona
  * #### Descripción del problema que soluciona
  El programa permite calcular la edad exacta de una persona, mediante el ingreso de la fecha de nacimiento del usuario (dd/mm/yy) y el ingreso de la fecha actual (dd/mm/yy).
  * #### Funcionalidad
  En este programa, solo vamos a usar variables de tipo entero (`int`).
  
  Para iniciar el programa, tenemos que ingresar el valor de las variables que van a representar la fecha actual, bajo el formato día/mes/año (`jm_dd`, `jm_mm` y `jm_yy` respectivamente).
  
  A continuación, se tiene que ingresar el valor de las variables que van a representar la fecha de nacimiento del usuario, bajo el formato día/mes/año (`jm_dd1`, `jm_mm1`, `jm_yy1` respectivamente).
  
  Una vez que se ingresan esas variables, el programa va a realizar dos operacions lógicas, usando la función `if`; la primera de ellas, va a estar compuesta por los siguientes procesos:
  
En caso de que el dia actual ingresado, sea menor al dia de nacimiento del usuario (`jm_dd<jm_dd1`):
  > `jm_dd=jm_dd+30;` (Se suman 30 dias al día actual ingresado por el usuario).
  > 
  > `jm_mm=jm_mm-1;` (Se resta un mes a la cantidad de meses ingresados por el usuario).
  > 
  > `jm_da=jm_dd-jm_dd1` (Usamos la variable `jm_da`, que va a almacenar la diferencia entre el día actual y el día de nacimiento).
  > 
_Si no se cumple esa condición (`jm_dd<jm_dd1`), entonces simplemente se produce la diferencia entre el día actual, y el día de nacimiento, almancenado en la variable `jm_da` (`jm_da=jm_dd-jm_dd1`)._

En caso de que el mes actual ingresado, sea menor al mes de nacimiento del usuario (`jm_mm<jm_mm1`):
  >`jm_mm=jm_mm+12;` (Se suman 12 meses a la cantidad de meses actuales ingresados por el usuario).
  >
  >`jm_yy=jm_yy-1;` (Se quita un año a la cantidad de años actuales ingresados).
  >
  >`jm_ma=jm_mm-jm_mm1;` (Usamos la variable `jm_ma`, que va a almacenar la diferencia entre el mes actual y el mes de nacimiento).
  >
 _Si no se cumple esta condición (`jm_mm<jm_mm1`), entonces simplemente se produce la diferencia entre el mes actual, y el mes de nacimiento, almacenado en la variable `jm_ma` (`jm_ma=jm_mm-jm_mm1;`)._
 
Una vez culminados esos procesos, en la variable `jm_ya`, vamos a almacenar la diferencia entre el año actual ingresado, y el año de nacimiento del usuario (`jm_ya=jm_yy-jm_yy1`).
  * #### Salida
  Una vez que se realicen todos los procesos descritos antes, el programa imprime los siguientes resultados:
  > `jm_ya` (Esta variable almacena la diferencia entre el año actual y el año de nacimiento).
  > 
  > `jm_ma` (Esta varible almecena la diferencia entre el mes actual y el mes de nacimiento).
  > 
  > `jm_da` (Esta variable almacea la diferencia entre el día actual y el día de nacimiento).

  > Imagen de referencia:
  > 
  > ![laedad](https://github.com/josemm0505/Practica1/blob/main/Codigo_laedad.jpg)
  ### Programa contador y clasificador de monedas
  * #### Descripción del problema que soluciona
  El programa permite ingresar la cantidad de monedas que el usuario desee, repartidas en tres denominaciones (10, 25 y 50 centavos). Una vez ingresadas las monedas, el programa debe clasificar cuantas monedas de cada tipo se han ingresado, imprimir ese dato e imprimir el valor total del dinero ingresado.
  * #### Funcionalidad
  Este programa solo va a utilizar variables de tipo entero (`int`).
  
  Para comenzar con la realización del programa, debemos de usar la variable `jm_n` para que el usuario ingrese la cantidad de monedas a ingresar. Esta misma variable va a ser usada para determinar el tamaño del vector `num`, que vamos a declarar después.
  
  Una vez que hemos usado la variable `jm_n`, vamos a usar un vector de una dimensión, con el valor almacenado en la variable `jm_n` (`num [jm_n]`).
  
  Posterior a ello, vamos a usar la variable `jm_i`, con la cual el usuario tiene que ingresar los valores, con los cuales va a rellenar el vector declarado anteriormente.
  
  Adicional a esto, vamos a usar el buclue `for`, que va a permetir que el proceso anterior se repita hasta que se cumplan ciertas condiciones (`for (int jm_i=0; jm_i<jm_n; jm_i++)`).
  
  Complementando el programa, vamos a añadir la función `if` y `else_if` para poder analizar los tipos de monedas ingresadas por el usuario; en caso de que la moneda ingresada sea de un valor de 10 centavos(`num [jm_i]==10`), vamos a usar un acumulador (`jm_sum1`) que va a almacenar unicamente la cantidad de monedas de 10 centavos ingresadas.
  
  En caso de que la condición anterior no se cumpla, usaremos un `else_if`, en donde, si el valor de la moneda ingresada es de 25 centavos (`num [jm_i]==25`), vamos a usar un acumulador (`jm_sum25`) que va a almacenar unicamente la cantidad de monedas de 25 centavos; en caso de que no cumplan ninguna de las dos condiciones anteriores, usaremos un contador (`jm_sum50`) que va almacenar unicamente la cantidad de monedas de 50 centavos ingresadas.
  
  También, vamos a usar una variable (`jm_sum`) para almacenar la suma de todas las monedas ingresadas.
  * #### Salidas
  Una vez que se realicen los procesos descritos antes, el programa va a imprimr los siguientes resultados:
  > `jm_sum50` (Esta variable va a almacenar la cantidad de monedas de 50 centavos ingresadas).
  > 
  > `jm_sum25` (Esta variable va a almacenar la cantidad de monedas de 25 centavos ingresadas).
  > 
  > `jm_sum1` (Esta variable va a almacenar la cantidad de monedas de 10 centavos ingresadas).
  > 
  > `jm_sum` (Esta variable va a almacenar la sumatoria del valor de las monedas ingresadas).
  
  > Imagen de referencia:
  > 
  > ![CuentaMoneda](https://github.com/josemm0505/Practica1/blob/main/Codigo_CuentaMoneda.jpg)
 ## Descargar e instalar los programas
 Para poder descargar el repositorio en el que se encuentran los programas descritos en este post, tienes que realizar el siguiente proceso:
 ### Clonar el repositorio
 Para clonar el repositorio en tu entorno de trabajo, debes usar el comando `git clone`, seguido de la dirección del repositorio en donde se encuentra el trabajo.
 > `git clone https://github.com/josemm0505/Actividad-E2.git`
 
 Una vez clonado en tu equipo, tienes que usar el comando `git pull` para poder descargar cualquier cambio que se haya podido realizar en el repositorio.
 
 Usando el comando `ls` de termux, puedes verificar que se encuentran todos los archivos que acabas de descargar.
 
 _En caso de que necesites realizar y subir cambios en losp programas, recuerda usar los comandos `git status` (para ver que es lo que se somete a cambios), `git add` (para añadir esos cambios a la nube), `git commit` (para comentar esos cambios) y `git push` (para poder subir a github los cambios que introduciste)._
 
 ### Compilar los programas
 En caso de que desees compilar y correr los archivos `.cpp`, debes usar el comando `g++ nombre_del_programa.cpp -o nombre_del_programa`.
 _Ejemplo_
 
 >`g++ MejiaJose_Compara.cpp -o MejiaJose_Compara`

Gracias por leer <3
