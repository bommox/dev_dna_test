# Ejercicio de Recruiting: Análisis Básico de Genotipado

## Descripción del Ejercicio

En este ejercicio, trabajarás con archivos de genotipado en formato CSV para calcular métricas básicas relacionadas con la calidad y la distribución de variantes genéticas. No necesitas conocimientos previos en genética, solo habilidades de programación y manipulación de datos.

## Archivos Proporcionados

En la carpeta `input`, encontrarás varios archivos de genotipado (`.csv`) para que pruebes tu solución. Todos los archivos tienen el siguiente formato:

| RSID         | CHR  | POSITION   | GENOTYPE |
|--------------|------|------------|----------|
| rs123        | 1    | 123456     | AA       |
| rs456        | 2    | 789012     | AG       |
| rs789        | 1    | 234567     | --       |
| ...          | ...  | ...        | ...      |

### Definición de Columnas:
- **RSID**: Identificador único de una variante genética.
- **CHR**: Número del cromosoma.
- **POSITION**: Posición en el cromosoma.
- **GENOTYPE**: Genotipo asociado con la variante genética (puede ser `AA`, `AG`, `GG`, etc., o `--` para indicar datos faltantes).

## Tareas

1. **Leer los archivos:**  
   Escribe un script que procese los archivos CSV de la carpeta `input`.

2. **Cálculo del Call Rate:**  
   - El **Call Rate** mide la proporción de variantes con un genotipo válido (distinto de `--`).  
     Fórmula:  
     \[
     Call\ Rate = \frac{\text{Número de variantes con genotipo válido}}{\text{Número total de variantes}} \times 100
     \]
   - Imprime el resultado en un formato legible (por ejemplo: `Call Rate: 98.5%`).

3. **Distribución de Variantes por Cromosoma:**  
   - Cuenta cuántas variantes hay para cada valor de `CHR`.
   - Imprime el resultado como una lista o tabla simple. Ejemplo:  
     ```
     Variantes por cromosoma:
     Cromosoma 1: 1500
     Cromosoma 2: 1200
     ...
     ```

4. **Exportar Resultados:**  
   - Guarda los resultados en un archivo `resumen.txt` con el siguiente formato:
     ```
     Call Rate: 98.5%
     
     Variantes por cromosoma:
     Cromosoma 1: 1500
     Cromosoma 2: 1200
     ...
     ```

5. **Output Adicional (Opcional):**  
   Si consideras que hay otros resultados relevantes o formas de presentar los datos, inclúyelos en tu solución.

## Entrega

1. **Repositorio en GitHub:**  
   Sube tu solución a un repositorio público de GitHub que contenga:
   - El script que resuelve el ejercicio.
   - El archivo `resumen.txt` con los resultados generados.
   - Un archivo `README.md` con:
     - Instrucciones para ejecutar tu script.
     - Breve explicación de cómo calculaste el Call Rate y las variantes por cromosoma.
   - (Opcional) Otros outputs que consideres relevantes.


## Evaluación

- **Call Rate correcto:** El cálculo debe ser preciso.
- **Distribución por cromosoma correcta:** Los valores deben reflejar los datos proporcionados.
- **Uso del repositorio de GitHub:** Se valorará la organización, claridad en la estructura y documentación del proyecto.
- **Creatividad:** Se apreciarán outputs adicionales o mejoras en la presentación de los resultados.

---

¡Buena suerte!
