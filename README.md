# SarahG
Tarea 1 Progra
# Programa: Ejercicio10.py
# Objetivo: Ejercicio 10
# Autor: Sarah Gómez
#(Fórmula de Cardano) Crear un programa que reciba los coeficientes de un poligono de
# x^3 +a1x^2+a2x+a3=0, donde el ceoficiente x^3 es 1.
import math

#Primero hay que calcular unas cantidades
#Pedimos al usuario que ingrese los valores de los coeficientes
e= float(input("Ingrese el valor de a1: "))
f= float(input("Ingrese el valor de a2:"))
g= float(input("Ingrese el valor de a3: "))
x1=1
#Hacemos las cuentitas
h=9
Q = (((3*f)-(e**2)) / h)
R = ((9*e*f - 27*g - 2*(e**3))/54)
D=(Q**3) + (R**2)
#Imprimimos las raices con las desigualdades
if D >0:
    #Calculamos S1 y S2
    S1=((((Q**3)+(R**2))**(1/3))+ R)**(1/3)
    S2 =((((Q ** 3) - (R ** 2)) ** (1 / 3)) + R) ** (1 / 3)
    #Calculamos la raiz real
    x1= S1 + S2 -(e/3)
    #Calculamos las raices imaginarias
    x2= -((S1 + S2)/2) - (e/3) + (3**(1/2)/2)*(S1 - S2)
    x3 = -((S1 + S2)/2) - (e/ 3)- (3 ** (1 / 2) / 2) * (S1 - S2)
    print("Una de las raices es real y dos de ellas son complejas")
    #Vemos lo que pasa con los otros dos casos
elif D == 0:
    print("Todas las raices son reales y al menos dos son iguales")
elif D<0:
    print("Todas las raices son reales y distintas")

#programa: Ejercicio 7
#Author: Sarah Gómez
import math
print("(Tronco de cono) Crear un programa en Python que permita calcular el volumen de un tronco de cono")
#Para calcular el volumen de un cono necesitamos primero calcular la base, esa la asigna el usuario
#Le pedimos al usuario que ingrese el radio del cono
r = float(input("Ingresa el radio del cono: "))
B = (r**2)*math.pi
print("Base del cono:")
print(B)
#Ya que tenemos la base, solo multiplicamos por la altura del cono, de igual forma, dejamos que el usuario la ingrese
h = float(input("Ingresa altura del cono: "))
#multiplicamos el radio y la altura y dividimos entre 3
volumen = (B*h)/3
print("El volumen del cono es: ")
print(volumen)

    
