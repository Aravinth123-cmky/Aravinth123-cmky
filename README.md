def fibonacci_generator():
    a, b = 0, 1
    while True:
        yield a
        a, b = b, a + b

# Example: Print first 10 Fibonacci numbers
fib = fibonacci_generator()
for _ in range(10):
    print(next(fib))
