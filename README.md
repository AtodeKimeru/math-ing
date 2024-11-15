# math-ing

## Conectividad Turística Sostenible en Medellín

## Proyecto para UN Datathon 2024

### Descripción del Proyecto

Es un proyecto piloto desarrollado para la UN Datathon 2024 que tiene como objetivo visualizar y analizar la conectividad actual entre puntos turísticos de Medellín a través de la red de ciclovías. Este proyecto busca identificar oportunidades para mejorar la red de transporte sostenible orientada al turismo en la ciudad.

### Objetivos

- Crear un modelo de nodos que relacione los puntos turísticos de Medellín.
- Desarrollar una visualización en ArcGIS que destaque la conectividad turística a través de ciclovías en la ciudad.
- Proporcionar una base para futuras mejoras en la infraestructura de transporte sostenible para turistas.

### Alcance

El alcance actual del proyecto incluye:

1. La creación de un modelo de nodos que representa la conectividad entre puntos turísticos.
2. Un mapa interactivo en ArcGIS que visualiza esta conectividad en el contexto de la ciudad de Medellín.

### Equipo

Nuestro equipo está compuesto por:

- Juan Sebastián Sánchez
- Iván Camilo Barragán
- Santiago Villarreal

Contamos con el apoyo de:
- María Gilma (Brasil)

### Tecnologías Utilizadas

- Python (NetworkX, Matplotlib, Pandas)
- ArcGIS para visualización geoespacial
- Jupyter Notebooks para análisis de datos
- AWS sagemaker para crear la instancia de jupyterLab y conectar con los dataframes en el bucket
- AWS S3 para almacenar los dataframes en un bucket en S3
- AWS IAM para orquestar y gestionar permisos entre servicios

### Cómo Ejecutar el Proyecto

El modelo de grafos se ejecuta y visualiza desde jupyterLab en el archivo data_connection.ipynb
El mapa con todos los datos cargados de la ciudad de Medellín se ejecutó desde ArcGis map

### Resultados y Visualizaciones

Matriz de Adyacencia:
```
[[0 1 0 0 0 0 0 0 0]
 [1 0 1 1 1 1 1 1 1]
 [0 1 0 0 0 0 1 0 0]
 [0 1 0 0 0 0 0 0 0]
 [0 1 0 0 0 1 1 0 1]
 [0 1 0 0 1 0 0 0 1]
 [0 1 1 0 1 0 0 0 1]
 [0 1 0 0 0 0 0 0 0]
 [0 1 0 0 1 1 1 0 0]]

Número de nodos: 9
Número de aristas: 14

Grado de cada nodo:
Casa Museo Maestro Pedro Nel Gómez: 1
Centro de Desarrollo Cultural de Moravia: 8
Jardín Botánico Joaquín Antonio Uribe: 2
Jardín Morro de Moravia: 1
Museo Cementerio San Pedro: 4
Parque de los Deseos: 3
Parque Explora: 4
Parque Norte J. Emilio Valderrama: 1
Planetario Municipal de Medellín Jesús Emilio Ramírez González: 4

Nodo con el grado más alto: Centro de Desarrollo Cultural de Moravia (Grado: 8)

Densidad del grafo: 0.3889
```
![Conexión grafos](images/nodos.png)

![Mapa de ciclovías](images/map_arcgis.png)

### Próximos Pasos

- Integrar los modelos
- Integrar datos en tiempo real de uso de ciclovías.
- Expandir el modelo para incluir más puntos de interés turístico.
- Desarrollar recomendaciones específicas para mejoras en la infraestructura.


### Agradecimientos

Queremos expresar nuestro agradecimiento a todas los organizadores de UN Datathon 2024:

- Naciones Unidas (UN) por la organización y patrocinio del evento.
- Departamento Administrativo Nacional de Estadística (DANE) por proporcionar datos valiosos y apoyo.
- Ruta N por su apoyo en innovación y tecnología.
- Amazon Web Services (AWS) por proporcionar la infraestructura en la nube y herramientas necesarias.
- Esri por el acceso a las herramientas de ArcGIS para nuestras visualizaciones geoespaciales.
- Y a los demás organizadores y colaboradores.

Agradecemos también a todos los mentores, jueces y participantes que contribuyeron con su tiempo y experiencia para hacer de esta Datathon un evento enriquecedor y productivo.

