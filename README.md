# DS1307
Libreria para el Reloj En Tiempo Real DS1307 -CREATVRA -

Las siguientes son las funciones que trae la libreria:


1.	iniciar_ds1307(); 

Inicia la librería y las configuraciones necesarias para usar el reloj.
 

2.	" programar(int, int, int, int, int, int, int); " 

Esta función es la que programa el tiempo en el reloj. El formato de la hora esta en 24h. los días de la semana se programan en la variable WDIA, comenzando con el domingo como día # 1, lunes día # 2 y así sucesivamente. DIA2 indica los días del mes.
Esta función retorna un valor Booleano “true” si la programación fue exitosa y retorna un valor “false” si la programación no se realizó adecuadamente. Los valores se deben escribir en el siguiente orden:
  
          programar(int SEGUNDO, int MINUTO, int HORA, int WDIA, int DIA2, int MES, int AÑO);
          
 

3.	" programar_hora(int, int, int); "

Esta función programa solamente los segundos, minutos y hora en el reloj.

Esta función retorna un valor Booleano “true” si la programación fue exitosa y retorna un valor “false” si la programación no se realizó adecuadamente. Los valores se deben escribir según el siguiente orden:

          programar_hora(int SEGUNDO, int MINUTO , int HORA);
          
          

4.	" test_ds1307(); "

Esta función hace un test del Reloj para saber si está correctamente instalado o si está dañado.  Devuelve un valor booleano “false” si no se obtuvo comunicación con el reloj y retorna un valor “true” si el sensor está correctamente instalado.

          boolean TEST = test_ds1307();
          
 
5.	" leer_segundo(); " 

Esta función recibe los segundos almacenados en el reloj y los guarda en una variable “byte”
 
          byte SEGUNDO = leer_segundo();
          

6.	" leer_minuto(); " 

Esta función recibe los minutos almacenados en el reloj y los guarda en una variable “byte”

          byte MINUTO = leer_minuto();
 

7.	" leer_hora(); " 

Esta función recibe la hora almacenada en el reloj y lo guarda en una variable “byte”

          byte HORA = leer_hora();
 

8.	" leer_wdia(); " 

Esta función recibe el día de la semana almacenado en el reloj y lo guarda en una variable “byte”

          byte DIA_DE_SEMANA = leer_wdia();
 

9.	" leer_dia(); " 

Esta función recibe el día del mes almacenado en el reloj y lo guarda en una variable “byte”

          byte DIA_DEL_MES = leer_dia();
 

10.	" leer_mes(); "

Esta función recibe el mes almacenado en el reloj y lo guarda en una variable “byte”
  
          byte MES = leer_mes();
 

11.	" leer_year(); " 

Esta función recibe el año almacenado en el reloj y lo guarda en una variable “byte”

          byte YEAR = leer_year();

