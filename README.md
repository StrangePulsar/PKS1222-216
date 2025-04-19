# Modelado físico del blázar PKS 1222+216 con agnpy y Sherpa

## Descripción

Este proyecto aborda el análisis del blázar **PKS 1222+216**, una galaxia activa con un jet relativista orientado hacia la Tierra. Utilizando el modelo físico provisto por la librería `agnpy`, se simula su espectro de energía (SED), considerando los procesos de emisión más relevantes:

- Radiación sincrotrón generada por electrones relativistas en un campo magnético.
- Compton Inverso de tipo Synchrotron Self-Compton (SSC), donde los fotones sincrotrón son dispersados por los mismos electrones que los generaron.
- Compton Inverso externo (EC), considerando fotones provenientes del torus de polvo que rodea el núcleo activo.

El modelo se ajusta a datos observacionales utilizando el paquete `Sherpa`, permitiendo obtener una estimación coherente de los parámetros físicos del jet.

## Objetivos

- Construir un modelo físico del SED de PKS 1222+216 utilizando `agnpy`.
- Incluir los procesos de sincrotrón, SSC y EC con un dusty torus.
- Ajustar parámetros como el campo magnético, el Doppler factor, y la distribución de electrones a datos observacionales reales.
- Analizar la influencia de cada parámetro en la forma del espectro.

## Contenido del Notebook

1. **Importación de librerías y configuración inicial**: Preparación del entorno con `agnpy`, `sherpa`, `numpy` y `matplotlib`.
2. **Definición del modelo físico**:
   - Geometría del blob y parámetros del jet.
   - Parámetros físicos del torus de polvo y su interacción con el jet.
3. **Construcción del SED**: Cálculo de las componentes sincrotrón, SSC y EC.
4. **Carga de datos observacionales**: Incluye puntos reales del espectro del blázar.
5. **Fitting con Sherpa**: Ajuste de parámetros físicos a los datos.
6. **Visualización de resultados**: Comparación entre el modelo ajustado y los datos.

## Instrucciones de Uso

### Requisitos previos

- Python 3.8 o superior.
- Entorno Jupyter Notebook recomendado.

### Dependencias

- `agnpy`
- `sherpa`
- `numpy`
- `matplotlib`
- `astropy`

Se pueden instalar con:

```bash
pip install agnpy sherpa numpy matplotlib astropy
