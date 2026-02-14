# Programacion-3

import math

print ("Bienvenido al menu")
print ("1. Sumar")
print ("2. Restar")
print ("3. Multiplicar ")
print ("4. Dividir ")
print ("5. Funciones trigonometricas ")
print ("6. Raiz enesima ")
print ("7. Potencial enesima ")
print ("8. Factorial")
print ("9. Fibonacci ")
print ("10. Mínimo común múltiplo de 2 números")
print ("11. Maximo comun divisor de 2 numeros")
print ("12. IVA")

Opcion = input ("Escoja la opcion que desee ")

if Opcion == "1":

    print ("Bienvenido a la suma")
    Numero1 = int (input("Ingrese el primer numero : " ))
    Numero2 = int (input("Ingrese el segundo numero : "))
    Suma = Numero1 + Numero2
    print ("La suma de los dos numeros es : ", Suma)

elif Opcion == "2":

    print ("Bienvenido a la resta")
    Numero1 = int (input("Ingrese el primer numero : " ))
    Numero2 = int (input("Ingrese el segundo numero : "))

    Resta = Numero1 - Numero2
    print ("La resta de los dos numeros es : ", Resta)

elif Opcion == "3":

    print ("Bienvenido a la Multiplicacion")
    Numero1 = int (input("Ingrese el primer numero : " ))
    Numero2 = int (input("Ingrese el segundo numero : "))

    Multiplicacion = Numero1 * Numero2
    print ("La Multiplicacion de los dos numeros es : ", Multiplicacion)

elif Opcion == "4":

    print ("Bienvenido a la divicion")
    Numero1 = int (input("Ingrese el numero que desea dividir: " ))
    Numero2 = int (input("Ingrese el numero por el que desea dividir : "))

    if Numero2 == 0:

        print ("Error. NO ES POSIBLE LA DISION POR 0")
    else:
        Divicion = Numero1 / Numero2 
        
    print ("La Divicion de los dos numeros es : ", Divicion)

elif Opcion == "5":

    print ("Bienvenido a las funciones trigonometricas")
    print("Menu de funciones trigonometricas.")
    print ("1. Seno")
    print ("2. Coseno")
    print ("3. Tangente ")

    OpcionT = input("Menu de funciones trigonometricas.")

    if OpcionT == "1":

        print ("Bienvenido a la funcion trigonometrica Seno.")
        Numero1 = int (input("Ingrese el numero que desea conocer con la funcion seno : " ))

        Senx = math.sin (Numero1)
        print ("La funcion seno del numero " , Numero1 , " es : ", Senx)

    elif OpcionT == "2":

        print ("Bienvenido a la funcion trigonometrica Coseno. ")
        Numero1 = int (input("Ingrese el numero que desea conocer con la funcion coseno : " ))

        Cosx = math.cos (Numero1)
        print ("La funcion coseno del numero " , Numero1 , " es : ", Cosx)

    elif OpcionT == "3":

        print ("Bienvenido a la funcion trigonometrica Tangente ")
        Numero1 = int (input("Ingrese el numero que desea conocer con la funcion tangente : " ))

        Tanx = math.tan (Numero1)
        print ("La funcion tangente del numero", Numero1 , "es :", Tanx)

    else :
        print ("OPCION NO DISPONIBLE")

elif Opcion == "6":

    print ("Bienvenido a la Raiz Enesima ")
    Numero1 = int (input("Ingrese el numero que desea conocer la raiz enesima : " ))

    R1 = int (input ("Ingrese la raiz del numero : "))
    Raiz1 = Numero1 ** (1/R1)
    print ("La raiz ", R1, "del numero", Numero1, "es : ", Raiz1)


elif Opcion == "7":

    print ("Bienvenido a la opcion de potencial enesima.")
    Numero1 = int (input("Ingrese el numero que deseea elevar : " ))

    Poten1 = int (input("Ingrese la potencia a la cual quiere elevar el numero : "))
    Potencial1 = Numero1 ** Poten1
    print ("La potencia ", Poten1, "del numero ", Numero1 , " es : ", Potencial1)


elif Opcion == "8":

    print ("Bienvenido a la funcion Factorial")
    Numero1 = int (input ("Ingrese el numero que deseea conocer el factorial : "))

    Factorial1 = math.factorial(Numero1)
    print ("El factorial del numero ", Numero1, " es : ", Factorial1)

elif Opcion == "9":

    print ("Bienvenido a la funcion de fibonacci ")
    Fibo = int (input ("Ingrese el numero n de la escala de fibonacci que desea saber : "))
    
    def Fibonacci (n: int ):
        if n == 0:
            return 0
        if n == 1:
            return 1
        
        return Fibonacci (n-1) + Fibonacci (n-2)
    
    print ("El numero de fibonacci es : ", Fibonacci(Fibo))

    
elif Opcion == "10":

    print ("Bienvenido a la funcion Mínimo común múltiplo de 2 números")
    Numero1 = int (input ("Ingrese el primer numero : "))
    Numero2 = int (input ("Ingrese el segundo numero : "))

    MinimoComun = math.lcm (Numero1, Numero2)
    print ("El minimo comun multiplo de los numeros ", Numero1, ", ", Numero2, " es : ", MinimoComun)

elif Opcion == "11":

    print ("Bienvenido a la funcion maximo comun divisor ")
    Numero1 = int (input ("Ingrese el primer numero : "))
    Numero2 = int (input ("Ingrese el segundo numero : "))

    MaxComun = math.gcd (Numero1, Numero2)
    print ("El maximo comun divisor de los numeros ", Numero1, ", ", Numero2, " es : ", MaxComun)

elif Opcion == "12":

    print ("Bienvenido a la funcion de IVA ")
    Valor = float (input("Ingrese el valor al que desea colocar IVA : "))
    IVA = int (input("Ingrese el iva que desea (ejemplo 15) : "))

    IVAP = IVA / 100

    IVAT = Valor + (Valor*IVAP)

    print ("El iva ", IVA, "%", "del valor", Valor, "$" , " es : ", IVAT, "$")


else: 
    print ("OPCION NO DISPONIBLE")
