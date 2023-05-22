# pseint
//Logica de una operacion
Algoritmo ejercicio1	
Definir a,b,c,resultado como reales;
Escribir "Digite el valor de A: "; 
leer a
Escribir "Digite el valor de B: ";  
leer b;  
Escribir "Digite el valor de C: ";  
leer c; 
resultado <- (-b + rc(b^2 - 4*a*c))/(2*a);
Escribir "El resultado es: ",resultado;
FinAlgoritmo

//Solucion logica de operacion
Algoritmo ejercicio2
Definir a,b como reales; 
Definir resultado Como Logico;
Escribir "Digite el valor de a: ";
leer a;
Escribir "Digite el valor de b: "; 
leer b;
resultado <- ((3+5*8)<3 y ((-6/3*4)+2<2)) o (a>b);
escribir "El resultado es: ", resultado;
FinAlgoritmo
//Intercambiar variables
Algoritmo ejercicio3
Definir a,b,aux como enteros;
escribir "Digite el valor de a:";
leer a; 
escribir "Digite el valor de b: "; 
leer b;	
aux <- a;
a <- b;
b <- aux;
Escribir "El nuevo valor de a es: ",a;
Escribir "El nuevo valor de b es: ",b;
FinAlgoritmo
//Calcular la cantidad de segundos que están incluidos en el 
//número de horas, minutos y segundos ingresados por el usuario.
Algoritmo ejercicio4
	Definir horas, minutos,seg como enteros; 
    Definir horas_seg, minutos_seg, total_seg como enteros;
	Escribir "Digite las horas: ";
	Leer horas;
	Escribir "Digite los minutos: ";
	Leer minutos;
	Escribir "Digite los segundos: "; 
	Leer seg
	//Calcular el equivalente en segundos
	horas_seg <- horas * 3600;  
	minutos_seg <- minutos * 60;
	total_seg <- horas_seg + minutos_seg + seg;
	Escribir "Los segundos equivalentes son: ",total_seg;
FinAlgoritmo
// Hacer un programa para ingresar el radio de un circulo y se  
// reporte su área y la longitud de la circunferencia.
// area = pi* radio^2
// Longitud = 2 * pi * radio
Algoritmo ejercicio5

	Definir radio, area, lon como real; 
	Escribir "Digite el valor del radio:";  
	Leer radio;  
	area <- pi * radio^2;
	lon <- 2* pi * radio;
	Escribir "El area de la circunferencia es: ",area; 
	Escribir "La longitud es: ",lon;
FinAlgoritmo
// Un maestro desea saber que porcentaje de hombres y que 
// porcentaje de mujeres hay en un grupo de estudiantes.
Algoritmo ejercicio6
    Definir num_hombres, num_mujeres como enteros;
	Definir total_estudiantes como entero;
	Definir porcentajeH, porcentajeM como reales; 
	Escribir "Digite el numero de hombres: ";
	Leer num_hombres; 
	Escribir "Digite el numero de mujeres: ";
	Leer num_mujeres;
	total_estudiantes <- num_hombres+num_mujeres; 
	porcentajeH <- num_hombres / total_estudiantes * 100; 
	porcentajeM <- num_mujeres / total_estudiantes * 100;
	Escribir "El porcentaje de Hombres es: ", porcentajeH, "%"
	Escribir "El porcentaje de Mujeres es. ', porcentajeM, "%"
FinAlgoritmo
//Un profesor prepara tres cuestionarios para una evaluación final: 
//A, B y C. Se sabe que se tarda 5 minutos en revisar el cuestionario A, 
//8 en revisar el cuestionario B y 6 en el C. La cantidad de exámenes de cada  
//tipo se entran por teclado. ¿Cuántas horas y cuántos minutos se tardará en 
//revisar todas las evaluaciones?
Algoritmo ejercicio7
	Definir cantidadA, cantidadB, cantidadC como enteros; 
	Definir tiempoA, tiempoB, tiempoC como enteros;
	Definir tiempo_total como entero;
	Definir horas, minutos como entero;
	Escribir "Digite la cantidad de cuestionarios A: ";
	Leer cantidadA;
	Escribir "Digite la cantidad de cuestionarios B: ";
	Leer cantidadB;
	Escribir "Digite la cantidad de cuestionarios C: ";  
	Leer cantidadC;
	//Calcular los minutos que se tardara por cada cuestionario
	tiempoA <- cantidadA * 5;
	tiempoB <- cantidadB * 8;
	tiempoC <- cantidadC * 6;
	//Calculamos el tiempo total que le toma revisar todos los cuestionarios 
	tiempo_total <- tiempoA + tiempoB + tiempoC;
	//Calculamos las horas y minutos
	horas <- trunc(tiempo_total / 60);
	minutos <- tiempo_total mod 60;
	Escribir "Se tardara ",horas," horas y ",minutos," minutos"
FinAlgoritmo
// Una tienda ofrece un descuento del 15% sobre el total de la 
// compra y un cliente desea saber cuánto deberá pagar finalmente por su compra.
Algoritmo ejercicio8
	Definir precio, descuento, precio_final como real;
	Escribir "Digite el precio a pagar: ";
	Leer precio;
	descuento <- precio*0.15;
	precio_final <- precio - descuento;
	Escribir "El precio a pagar es de: ", precio_final;
FinAlgoritmo
// Un alumno desea saber cuál será su calificación final en la materia de 
// Algoritmos. Dicha calificación se compone de los siguientes porcentajes:
// 55% del promedio de sus tres calificaciones parciales. 
// 30% de la calificación del examen final.
// 15% de la calificación de un trabajo final.
Algoritmo ejercicio9
	Definir parcial1, parcial2, parcial3, promedioP, notasParcial como reales
	Definir examen_final, notaExamen como reales 
	Definir notaTrabajo, notaFinalTrabajo como reales
	Definir notaFinal como real
	Escribir "Digite las 3 notas de los parciales"
	Leer parcial1,parcial2,parcial3
	promedioP <- (parcial1+parcial2+parcial3)/3
	notasParcial <- promedioP*0.55
	Escribir "Digite la nota del examen final:"
	Leer examen_final
	notaExamen <- examen_final * 0.3
	Escribir "Digite la nota del trabajo final:"
	Leer notaTrabajo
	notaFinalTrabajo <- notaTrabajo * 0.15
	notaFinal <- notasParcial+notaExamen+notaFinalTrabajo
	Escribir "La calificacion final es: ",notaFinal
FinAlgoritmo
//Ingrese un número entero y reportar si es par o impar.
Algoritmo ejercicio10
	Definir num como entero;
	Escribir "Digite un numero:"
	Leer num;
Si num mod 2 = 0 Entonces
	Escribir "El numero ",num," es par"; 
SiNo  
	Escribir "El numero ", num," es impar";  
FinSi
FinAlgoritmo
// Determinar si un alumno aprueba o reprueba un curso, sabiendo que
// aprobará si su promedio de tres calificaciones es mayor o igual a 70
// reprueba caso contrario. 
Algoritmo ejercicio11
	Definir nota1,nota2,nota3 como reales
		Definir prom como real
	Escribir "Digite las 3 calificaciones:"
	Leer nota1,nota2,nota3
	prom <- (nota1+nota2+nota3)/3
	Si prom>=70 Entonces
		Escribir "El alumno esta aprobado con: ",prom
	SiNo
		Escribir "El alumno esta desaprobado con: ",prom
	FinSi
FinAlgoritmo
//En un almacén se hace un 20 MOD  de descuento a los clientes 
// cuya compra supere los $100. ¿Cuál será la cantidad que pagará una 
// persona por su compra? 
Algoritmo ejercicio12
	Definir compra,precio_final como real
	Escribir "Digite la cantidad a pagar: "
	Leer compra
	Si compra>100 Entonces
		descuento <- compra * 0.2
	SiNo
		descuento <- 0
	FinSi
	precio_final <- compra - descuento
	Escribir "El precio a pagar es: ",precio_final
FinAlgoritmo
//Leer 2 numeros ;si son iguales que los multiplique, si el 
// primero es mayor que el segundo que los reste y si no que los sume.
Algoritmo ejercicio13
Definir num1,num2, resultado como reales;
	Escribir "Digite dos numeros: ";
	Leer num1,num2;
	Si num1=num2 Entonces
	    //Si son iguales multiplicamos
		resultado <- num1 * num2;
	SiNo
	     Si num1>num2 Entonces
			//Si el primer numero es mayor los restamos resultado <- num1 - num2;
			resultado <- num1 - num2; 
	SiNo
			resultado <- num1 + num2; 
	    FinSi
	FinSi
	Escribir "El resultado es: ", resultado;
FinAlgoritmo
// Leer tres números diferentes e imprimir 
// el número mayor de los tres.
Algoritmo ejercicio14
	Definir num1,num2,num3 como reales
	Escribir "Digite tres numeros diferentes: "
	Leer num1,num2,num3
	Si num1>num2 y num1>num3 Entonces
		Escribir "El mayor es: ",num1
	SiNo
		Si num2>num1 y num2>num3 Entonces
			Escribir "El mayor es: ",num2
		SiNo
			Escribir "El mayor es: ",num3
		FinSi
	FinSi
FinAlgoritmo
//Cuanto pagara una persona que compre manzanas con descuento x kilos
Algoritmo ejercicio15
	Definir preciok,kilos,precioI como reales
	Definir descuento,precio_final como reales
	Escribir "Cuanto cuesta el kilo de manzanas? "
	Leer preciok
	Escribir "Cuantos kilos de manzana a comprado? "
	Leer kilos
	precioI <- preciok * kilos
	Si kilos>=0 y kilos <=2 Entonces
		descuento <- 0
	SiNo
		Si kilos>=2.01 y kilos<=5 Entonces
			descuento <- precioI * 0.1
		SiNo
			Si kilos>=5.01 y kilos<=10 Entonces
				descuento <- precioI * 0.15
			SiNo
				descuento <- precioI*0.2
			FinSi
		FinSi
	FinSi
	precio_final <- precioI -  descuento
	Escribir "El precio a pagar es: $",precio_final
FinAlgoritmo
//Elaborar un programa que me muestre los días de las semanas 
// cuando ingrese Los siete primeros números.
Algoritmo ejercicio16
	Definir num como entero;
	Escribir "Digite un numero del dia de la semana (1-7): ";  
	Leer num;
	Segun num Hacer
		1:Escribir "Lunes";
		2:Escribir "Martes";
		3:Escribir "Miercoles";
		4:Escribir "Jueves";
		5:Escribir "Viernes";
		6:Escribir "Sabado";  
		7:Escribir "Domingo";
		De Otro Modo:
			Escribir "Error, no existe dia para ese numero";
	FinSegun
FinAlgoritmo
//Elaborar un programa que me muestre el 
//significado de aniversario de cada década hasta los 60.
Algoritmo ejercicio17
	Definir decada como entero
	Escribir "Digite una decada"
	Leer decada
	Segun decada Hacer
		10:
			Escribir "Bodas de Hojalata"
		20:
			Escribir "Bodas de Porcelana"
		30:
			Escribir "Bodas de Perlas"
		40:
			Escribir "Bodas de Rubi"
		50:
			Escribir "Bodas de Oro"
		60:
			Escribir "Bodas de Diamante"
		De Otro Modo:
			Escribir "Decada no existente"
	FinSegun
FinAlgoritmo
//Hacer un programa que tenga un menú con las siguientes opciones:
//Opción 1: Elevar un número a una potencia X
//Opción 2: Sacar la raíz cuadrada de un número
//Opción 3: Salir
Algoritmo ejercicio18
	Definir opcion Como Entero
	Escribir "MENU"
	Escribir "1. Elevar un numero a una potencia X"
	Escribir "2. Sacar la raiz cuadrada de un numero"
	Escribir "3. Salir"
	Escribir "Digite una opcion: "
	Leer opcion
	Segun opcion  Hacer
		1:
			Definir num,pot,resultado Como Real
			Escribir "Digite un numero: "
			Leer num
			Escribir "Digite la potencia"
			Leer pot
			resultado <- num^pot
			Escribir "El resultado es: ",resultado
		2:
			Definir num,resultado Como Real
			Escribir " Digite un numero: "
			Leer num
			resultado <- rc(num)
			Escribir "El resultado es: ",resultado
		3:
		De Otro Modo:
			Escribir "Se equivoco de opcion menu"
	FinSegun
FinAlgoritmo
//Calcular la suma de los "N" primeros números
Algoritmo ejercicio19
	Definir N, suma, i como entero;
	Escribir "Digite la cantidad de numeros a sumarse: ";
	Leer N;
	suma <- 0;
	Para i<-1 Hasta N Con Paso 1 Hacer
	   suma <- suma + i;
		
	FinPara
	Escribir"La suma es: ",suma;
FinAlgoritmo
//Se desea calcular independientemente la suma  
//de Los números pares e impares comprendidos entre 1 y 50.
Algoritmo ejercicio20
	Definir suma_pares,suma_impares,i como enteros
	suma_pares <- 0
	suma_impares <- 0 
	Para i<-2 Hasta 49 Hacer
		Si i mod 2 = 0 Entonces
			suma_pares <- suma_pares + i
		SiNo
			suma_impares <- suma_impares+i
		FinSi
	FinPara
	Escribir "La suma de pares es: ",suma_pares
	Escribir "La suma de impares es: ",suma_impares
FinAlgoritmo
//Leer 10 números e imprimir cuantos son positivos, 
// cuantos negativos y cuantos neutros.
Algoritmo ejercicio21
    Definir positivos, negativos, neutros, numero, contador como Entero
    
    positivos <- 0
    negativos <- 0
    neutros <- 0
    
    Para contador <- 1 Hasta 10 Hacer
        Escribir "Digite un número:"
        Leer numero
        
        Si numero > 0 Entonces
            positivos <- positivos + 1
        SiNo
            Si numero < 0 Entonces
                negativos <- negativos + 1
            SiNo
                neutros <- neutros + 1
            FinSi
        FinSi
        
    FinPara
    
    Escribir "Cantidad de números positivos:", positivos
    Escribir "Cantidad de números negativos:", negativos
    Escribir "Cantidad de números neutros:", neutros
    
FinAlgoritmo
//Suponga que se tiene un conjunto de calificaciones de un grupo 
//de 10 alumnos. Realizar un algoritmo para calcular la calificación promedio y 
// a calificación más baja de todo el grupo.
Algoritmo ejercicio22
	Definir calificacion_promedio,calificacion_baja como real; 
	Definir calificacion, suma como real;
	Definir i como entero;
	suma<-0;
	calificacion_baja<-9999;
	Para i<-1 Hasta 10 con Paso 1 Hacer
		Escribir i,". Digite una calificacion: "; 
		Leer calificacion;
		
			//Suma iterativa de las calificaciones
		suma <- suma + calificacion;	
		//Calculamos la menor calficacion
		Si calificacion < calificacion_baja Entonces
			calificacion_baja<- calificacion;
		FinSi
	FinPara
	calificacion_promedio<-suma/10;
	Escribir " La calificacion promedio es: ", calificacion_promedio;
	Escribir "La calificacion baja es: ",calificacion_baja;
FinAlgoritmo
//Calcular el factorial de un número 
//mayor o igual a 0.
Algoritmo ejercicio23
	Definir num como entero
	Definir i,factorial como enteros
	Repetir
		Escribir "Digite un numero: "
		Leer num
	Hasta Que num>=0
	i <- 1
	factorial <- 1 
	// N!=1*2*3*...*N
	Mientras i<=num Hacer
		factorial <- factorial * i
		i <- i+1
	FinMientras
	Escribir "El factorial es: ",factorial
FinAlgoritmo
//Calcular la siguiente sumatoria de los "N" elementos: 
//S = 1 + 4 + 9 + ...
Algoritmo ejercicio24
	Definir n_elementos como entero
	Definir i, suma como enteros
	Escribir "Digite la cantidad de elementos a sumarse: "
	Leer n_elementos
	i <- 1
	suma <- 0
	Mientras i<=n_elementos Hacer
		suma <- suma+i^2
		i <- i+1
	FinMientras
	Escribir "La suma es: ",suma
FinAlgoritmo
//Ingresar "N" enteros, visualizar la suma de los números pares 
//de la lista, cuántos números pares existen y cuál es el promedio de los numero impares
Algoritmo ejercicio25
	Definir n_elementos,i,num como enteros;
	Definir suma_pares,conteo_pares como enteros;
	Definir suma_impares,conteo_impares como enteros;
	Definir prom_impares como real;
	Escribir "Digite la cantidad de elementos a ingresar: ";
	Leer n_elementos;
	i<-1;
	suma_pares <-0;
	conteo_pares<-0;
	
	suma_impares<-0;
	conteo_impares<-0;
	Mientras i<= n_elementos Hacer 
		Escribir i,". Digite un numero: ";
		Leer num; 
		Si num mod 2 = 0  Entonces
			//El num es par
			suma_pares<-suma_pares+num;
			
			//Conteo de pares
			conteo_pares<-conteo_pares+1;
		SiNo
			//El num es impar
			
			//Suma iterativa de impares
			suma_impares<-suma_impares+num;
			
			//Conteo de impares
			conteo_impares<-conteo_impares+1;
		Fin Si
		i <- i + 1;
	FinMientras
	
	Si conteo_pares = 0 Entonces
		Escribir "No se han digitados numeros pares";
	SiNo
		Escribir "La suma de los numeros pares es: ",suma_pares;
		Escribir "El conteo de los numeros pares es: ",conteo_pares
	FinSi
	
	Si conteo_impares = 0 Entonces
		Escribir "No se han digitado numeros impares";
	SiNo
		prom_impares<-suma_impares/conteo_impares;
		Escribir "El promedio de impares es: ",prom_impares;
	FinSi
FinAlgoritmo
//Sacar las horas trabajadas de 5 perdsonas 
//La tarifa de pago 
//La sumatoria de todo los salarios
Algoritmo ejercicio26
    Definir horasTrabajadas, tarifaPago, salario, sumaSalarios Como Entero
    
    sumaSalarios <- 0
    
    Para i <- 1 Hasta 5 Hacer
        Escribir "Ingrese las horas trabajadas de la persona ", i, ": "
        Leer horasTrabajadas
        
        Escribir "Ingrese la tarifa de pago por hora de la persona ", i, ": "
        Leer tarifaPago
        
        salario <- horasTrabajadas * tarifaPago
        
        Escribir "El salario de la persona ", i, " es: ", salario
        
        sumaSalarios <- sumaSalarios + salario
        
        Escribir ""
    FinPara
    
    Escribir "La sumatoria de todos los salarios es: ", sumaSalarios
    
FinAlgoritmo
