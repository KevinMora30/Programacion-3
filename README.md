# Programacion-3
# Generar n números de Fibonacci
def fibonacci(n):
    a, b = 0, 1
    for _ in range(n):
        a, b = b, a + b
    return a
t=int(input())
print(fibonacci(t-1))
