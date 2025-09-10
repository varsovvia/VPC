# Proyecto de Visión por Computador

## ⚙️ Configuración del entorno en Visual Studio Code/Cursor

Este proyecto utiliza un entorno de **conda** llamado `practica_1_VPC` para ejecutar los notebooks.

### Pasos para configurarlo:

1. **Crear y activar el entorno**
   ```bash
   conda create -n practica_1_VPC python=3.11 -y
   conda activate practica_1_VPC
   ```

2. **Instalar las dependencias**
   ```bash
   conda install -c conda-forge numpy matplotlib opencv ipykernel jupyter -y
   ```

3. **Registrar el kernel en Jupyter**
   ```bash
   python -m ipykernel install --user --name practica_1_VPC --display-name "Python (practica_1_VPC)"
   ```

4. **Seleccionar el kernel en VSCode/Cursor**
   - Abre el archivo `.ipynb`
   - Arriba a la derecha: "Kernel → Select Kernel"
   - Escoge "Python (practica_1_VPC)"

5. **Probar la instalación**
   Ejecuta en una celda:
   ```python
   import sys, numpy, cv2, matplotlib
   print("Python:", sys.version)
   print("numpy:", numpy.__version__)
   print("opencv:", cv2.__version__)
   print("matplotlib:", matplotlib.__version__)
   ```

## Estructura del Proyecto

```
P_1/
├── 1_Intro_TranfXeom_Calib.ipynb    # Notebook principal
└── Images/                          # Imágenes para ejercicios
    ├── Intro_images/
    ├── Calibration_images/
    ├── Edge_images/
    └── ...
```

## Trabajo en Parejas

1. **Cada miembro:**
   - Clona el repositorio
   - Configura el entorno siguiendo los pasos anteriores
   - Trabaja en su propia rama

2. **Compartir cambios:**
   ```bash
   git add .
   git commit -m "Descripción de los cambios"
   git push origin nombre-rama
   ```