Carpeta Instances
Contiene los clientes tomados de forma aleatoria de la base de datos de la Multinacional. Este documento se organiza en el siguiente orden:

1.) Número de nodos en total incluyendo el depósito

Paámetros del depósito
2.) Coordenada X = 0 (cm) ; Coordinadas Y=0 (cm) ; Demanda=0 (cajas) ; Tiempo de servicio=0 (min) ; Tipo de nodo (line 1 /back 0 ) =0 ; Límite inferior TW=0 (min) ; Límite superior TW=1440 (min todo el día) 

Parámetros de cada cliente
3.) Coordenada X (cm) ; Coordinadas Y (cm) ; Demanda (cajas) ; Tiempo de servicio (min) ; Tipo de nodo (line 1 /back 0 ) ; Límite inferior TW (min) ; Límite superior TW (min)

Al final de todos los clientes 
4.) Matriz de variaciones de un nodo a otro: establecimos 5%, 15% y 25%



////////////////////////////

Carpeta Dats
Contiene los archivos .dat de las instancias determinista

param V1= cantidad de clientes;
param COST_cm=0.00451414 Costo por centimetro recorrido (COP);
param COST_min=2000 costo por minuto recorrido (COP);
param K1= cantidad de vehiculos;
param M=9000000 (GRAN M);
param CV= costo de utilización del vehículo (COP);
param U=2 capacidad del vehículo (cajas);
param Dem:= demanda de los clientes (cajas)
;

param a:= límite inferior TW (min)
;

param b:= límite superior TW (min)
;

param s: tiempo de servicio (min)
;

param D: matriz de distancias de un nodo a otro (cm)
;

param t: matriz de tiempos de viaje de un nodo a otro (min)


////////////////////////////

Carpeta Escenarios
Contiene los archivos .dat con el componenete estocástico

param N= cantidad de escenarios;
param V1= cantidad de clientes;
param COST_cm=0.00451414 Costo por centimetro recorrido (COP);
param COST_min=2000 costo por minuto recorrido (COP);
param K1= cantidad de vehiculos;
param FC=83333.3; //factor de conversión que no se utilizó pero que se agregó a los archivos
param M=9000000 (GRAN M);
param CV= costo de utilización del vehículo (COP);
param U=2 capacidad del vehículo (cajas);
param Dem:= demanda de los clientes (cajas)
;

param a:= límite inferior TW (min)
;

param b:= límite superior TW (min)
;

param s: tiempo de servicio (min)
;

param D: matriz de distancias de un nodo a otro (cm)
;

param t: matriz de tiempos de viaje de un nodo a otro (min)

param E:= matriz de tiempos por cada escenario
[*,*,1]:
