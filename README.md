# Programacion-3
# Generar n números de Fibonacci
def fibonacci(n):
    a, b = 0, 1
    for _ in range(n):
        a, b = b, a + b
    return a
t=int(input())
print(fibonacci(t-1))

#Calcular el iva de un producto
def IVA(n, r):
    Val=n+n*(r/100)
    return Val
print("Digite el precio del producto")
n=int(input())
print("Digite el IVA del producto")
r=float(input())
print(IVA(n, r))
