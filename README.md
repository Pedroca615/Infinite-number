# infinite_generator.py

def generate_infinite_numbers():
    num = 0
    while True:
        yield num
        num += 1

# Função para testar a geração de números
if __name__ == "__main__":
    generator = generate_infinite_numbers()
    for _ in range(10):  # Imprime os primeiros 10 números
        print(next(generator))
