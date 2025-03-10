# -promedio_temperaturas.py-
import random

# Configuración de la matriz 3D
ciudades = ["Ciudad A", "Ciudad B", "Ciudad C"]
dias = ["Lunes", "Martes", "Miércoles", "Jueves", "Viernes", "Sábado", "Domingo"]
semanas = 2  # Número de semanas

# Crear la matriz 3D (ciudades x semanas x días) y llenarla con temperaturas aleatorias
temperaturas = [[[random.randint(15, 35) for _ in dias] for _ in range(semanas)] for _ in ciudades]

# Calcular y mostrar el promedio de temperaturas para cada ciudad por semana
for i, ciudad in enumerate(ciudades):
    print(f"\n--- {ciudad} ---")
    for j in range(semanas):
        total = sum(temperaturas[i][j])
        promedio = total / len(dias)
        print(f"Semana {j + 1}: Promedio de temperatura = {promedio:.2f}°C")



        # Inicializa el repositorio local
git init

# Agrega el archivo
git add promedio_temperaturas.py

# Crea un commit
git commit -m "Añadir script para cálculo de promedios de temperatura"

# Conecta tu repositorio local con el remoto
git branch -M main
git remote add origin https://github.com/TU_USUARIO/promedio-temperaturas-ciudades.git

# Sube los cambios
git push -u origin main


la excelencia no es un acto es un habito
