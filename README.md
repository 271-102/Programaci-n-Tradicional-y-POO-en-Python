# Programaci-n-Tradicional-y-POO-en-Python
casandra muyolema 
# Programa: Promedio de temperatura semanal (Tradicional)

def ingresar_temperaturas():
    temperaturas = []
    for i in range(7):
        temp = float(input(f"Ingrese la temperatura del día {i + 1}: "))
        temperaturas.append(temp)
    return temperaturas

def calcular_promedio(temperaturas):
    return sum(temperaturas) / len(temperaturas)

def mostrar_resultado(promedio):
    print(f"\nEl promedio semanal de temperaturas es: {promedio:.2f} °C")

# Programa principal
def main():
    print("== Promedio Semanal de Temperaturas (Tradicional) ==")
    temps = ingresar_temperaturas()
    promedio = calcular_promedio(temps)
    mostrar_resultado(promedio)

if __name__ == "__main__":
    main()
