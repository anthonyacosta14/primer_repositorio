# primer_repositorio
---
## Rutina de entrenamiento
---
### Básica
- uno: Curl de biceps 3 repeticiones
- dos: Curl martillo 3 repeticiones
- tres: Press mariposa 5 repeticiones muy suaves
- cuatro: Si quieres mas información sobre rutinas básicas ve a este a este [enlace](https://www.buff-academy.com/challenge-page/58b99aa7-547f-46fc-903a-5ecf38010b83?programId=58b99aa7-547f-46fc-903a-5ecf38010b83)
---
### Dificultad máxima
- uno: flexiones diamante 20 repeticiones
- dos: press militar 35 repeticiones
- tres: press banca 28 repeticiones
- cuatro: si quieres mas informaciones sobre rutinas complejas ve a este [enlace](https://www.buff-academy.com/challenge-page/782459a3-78c7-452b-859c-4397f8f5548f?programId=782459a3-78c7-452b-859c-4397f8f5548f)
---
## Códigos de crud
### CRUD sencillo
~~~
from domain.modelo.coche import Coche
from domain.servicios.cochesServicios import CochesServicios

def main():
    cochesServicios : CochesServicios = CochesServicios()
    while True:
        print(" 1. Crear coche")
        print(" 2. Listar coches")
        print(" 3. Buscar coche")
        print(" 4. Borrar coche")
        print(" 5. Salir")
        opcion = input("Introduce una opcion: ")
        if (opcion == "1"):
            matricula :str = input("dime la matricula")
            color :str = input("dime el color")
            marca :str = input("dime la marca")
            modelo :str = input("dime el modelo")
            coche_nuevo : Coche = Coche(matricula, marca, modelo, color)
            cochesServicios.crear_coche(coche_nuevo)
            print("Coche creado")           
        elif (opcion == "2"):
            coches : list[Coche] = cochesServicios.listar_coches()
            for coche in coches:
                print(coche)
        elif (opcion == "3"):
            print("TODO")
        elif (opcion == "4"):
            matricula :str = input("dime la matricula")
            cochesServicios.cambiar_coche(matricula)
        elif (opcion == "5"):
            break
        else:
            print("Opcion incorrecta")
~~~
## IMAGEN CURIOSA Y OBLIGATORIA
![imagen](/imagenes/imagenn.jpg)
![imagen](/imagenes/sergio.jpg)
