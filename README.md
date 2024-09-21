from rich.console import Console

# Clase Flor
class Flor:
    def __init__(self, color, tipo):
        self.color = color
        self.tipo = tipo

    def __str__(self):
        return f'{self.tipo} de color {self.color}'

# Clase Ramo
class Ramo:
    def __init__(self):
        self.flores = []

    def agregar_flor(self, flor):
        self.flores.append(flor)

    def mostrar_ramo(self):
        print("Ramo de flores:")
        for flor in self.flores:
            print(flor)

# Crear un objeto de Console para manejar la salida formateada
console = Console()

# Código principal
if __name__ == "__main__":
    ramo_de_flores = Ramo()

    # Añadiendo flores amarillas al ramo
    ramo_de_flores.agregar_flor(Flor("amarillo", "Rosa"))
    ramo_de_flores.agregar_flor(Flor("amarillo", "Girasol"))
    ramo_de_flores.agregar_flor(Flor("amarillo", "Tulipán"))

    # Mostrando el ramo de flores
    ramo_de_flores.mostrar_ramo()

    # Imprimir "Te amo Mishelle" en letra cursiva
    console.print("\nTe amo Mishelle", style="italic bold magenta")# FloresAmarillas
