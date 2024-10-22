# Generador de Datos Aleatorios de Empleados

Este proyecto tiene como objetivo generar un conjunto de datos aleatorios que simula la información de empleados en una empresa. El conjunto de datos incluye campos como nombre, apellido, edad, salario y departamento. Se utiliza la biblioteca `pandas` para crear y manipular el DataFrame, y la biblioteca `random` para generar valores aleatorios.

## Descripción del Funcionamiento

1. **Definición de Departamentos**: Se establece una lista de departamentos en los que los empleados pueden trabajar, como Recursos Humanos, Marketing, Ventas, IT, Finanzas, Producción, Investigación y Logística.

2. **Generación de Datos Aleatorios**: La función `generar_datos_empleados(num_registros)` toma como argumento el número de registros que se desean generar. Dentro de la función:
   - Se definen listas de nombres y apellidos.
   - Se generan listas aleatorias de edades (entre 22 y 60 años) y salarios (entre $20,000 y $120,000).
   - Se asigna aleatoriamente un departamento a cada empleado.
   - Se crea un DataFrame con los datos generados.

3. **Exportación a CSV**: El DataFrame resultante se guarda en un archivo CSV en una ubicación especificada.

### Ejemplo de Uso

Para utilizar este código, simplemente debes llamar a la función `generar_datos_empleados` con el número de registros que deseas generar. Por ejemplo:

```python
df_empleados = generar_datos_empleados(1000)
```

Este código generará un DataFrame con 1000 registros de empleados y lo guardará en un archivo CSV en la ruta especificada.

## Consideraciones

- Asegúrate de tener la biblioteca `pandas` instalada en tu entorno de Python. Puedes instalarla utilizando el siguiente comando:

  ```
  pip install pandas
  ```

- Modifica la ruta de `csv_path` para adaptarla a tu sistema de archivos, asegurándote de que la carpeta de destino exista.

## **Utilidad en Ingeniería de Datos**

**Este código es útil para la ingeniería de datos ya que permite simular grandes volúmenes de datos de empleados, lo que puede ser beneficioso en pruebas de rendimiento, desarrollo de pipelines de datos y análisis de datos. Al generar datos aleatorios, se pueden crear escenarios de prueba para validar algoritmos de análisis, explorar diferentes patrones y mejorar la calidad de los modelos de machine learning. Además, el manejo de datos en formato CSV facilita su integración en diversos sistemas y herramientas de análisis.**
