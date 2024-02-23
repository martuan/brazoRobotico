Brazo robótico antropomórfico con 4 modos de funcionamiento  
	1) Por defecto: rutina de trabajo hardcodeada  
 	2) Por instrucción: puerto serie (1 instrucción cada vez)  
  	3) Por rutina cargada: puerto serie (instrucciones multilínea)/bluetooth (instrucción individual)  
	4) Por Bluetooth (instrucción individual)  
 
	Modo de uso:
	Por puerto serie: 
		El caracter delimitador es el ';'.
		'H' para ir al home
		'R' para secuencia repetitiva
		'S' para cortar secuencia repetitiva y continuar con secuencias simples
		Ejemplo: A, S1, 10, 100, 1000
			A: comando accionar servo
			S1: servo 1
			10: movimiento positivo de 10 grados
			100, demora entre cada paso de 1 grado. Es decir, modifica la velocidad
			1000: demora luego de que se completó el movimiento
	Por Bluetooth:
		El caracter delimitador es el '\n'
		Solo acepta secuencias individuales, enviadas por botonera de la app
		La secuencia es igual a la del ejemplo anteriores
