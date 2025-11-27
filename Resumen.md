# Análisis de Calidad del Aire - La Florida/Macul, RM

## Descripción
Análisis de datos de calidad del aire del sistema SINCA para el sector sur-oriente de Santiago, específicamente las comunas de La Florida y Macul. Este proyecto identifica patrones de contaminación y evalúa riesgos para la salud pública.

## Objetivo
Analizar la evolución de contaminantes atmosféricos y estimar el riesgo sanitario para habitantes del sector, mediante datos del monitor ubicado en la Municipalidad de La Florida.

### Preguntas de Investigación
- Comparación de niveles de CO vs otros contaminantes
- Tendencias temporales de PM2.5 en últimos años
- Relación entre O3 y NOX
- Modelo predictivo de PM2.5
- Evaluación de riesgo sanitario por superación de normas

### Configuración de Datos
- Fuente: Sistema SINCA (sinca.mma.gob.cl)
- Monitor: Municipalidad de La Florida
- Contaminantes: PM2.5, PM10, CO, O3, NOX
- Período: [2010] - [2025]

### Audiencia Objetivo
- Ciudadanía general
- Autoridades ambientales
- Instituciones educativas y de salud

### Pre-requisitos
bash
Python 3.8+
Jupyter Notebook

### 1. Contexto y motivaciones:
La calidad del aire es un tema súper importante hoy en día, especialmente en Santiago, donde hay un montón de cosas que la empeoran. Por ejemplo, todos los autos que andan por la calle, las fábricas, la contaminación que a veces generamos nosotros mismos y hasta cómo es la ciudad geográficamente, hacen que tengamos niveles de contaminación súper altos en el aire. Por eso, nos pusimos a pensar en este tema tan actual y se nos ocurrió buscar una solución usando unos aparatos que monitorean la contaminación y que están conectados al SINCA.

En particular, nos enfocamos en unos dispositivos que están en la Municipalidad de La Florida. Estos aparatos están analizando la contaminación del aire y sus diferentes componentes en varias zonas de Chile. Elegimos este dispositivo porque la zona que monitorea también incluye una parte de Macul, donde está la Pontificia Universidad Católica de Chile. Como pasamos la mayor parte del tiempo ahí, nos preocupa mucho la calidad del aire que respiramos. Pensamos en todas las enfermedades respiratorias que podríamos contraer, que nos podrían llevar al hospital o, en el peor de los casos, a algo mucho más grave. Los altos niveles de contaminación son factores directos en la aparición y agravamiento de enfermedades respiratorias, cardiovasculares y alérgicas. En ese contexto, buscamos contribuir a la concientización ciudadana y a la toma de decisiones informadas por parte de organismos públicos como el Ministerio del Medio Ambiente, las municipalidades y los servicios de salud, promoviendo la generación de conocimiento basado en datos abiertos. Además, nos dimos cuenta de que la gente de La Florida y de las comunas cercanas, como la nuestra, también está expuesta a estos riesgos, lo que hace que este problema sea aún más relevante para la comunidad en general. Queremos contribuir a que la gente tome conciencia de lo importante que es respirar aire limpio y cómo esto afecta directamente nuestra salud y bienestar a largo plazo. Es un tema que nos toca de cerca y sentimos que podemos aportar con este proyecto.

Además, esperamos que este trabajo ayude a comprender cómo se comportan distintos contaminantes atmosféricos en el tiempo y qué implicancias tienen para la salud pública, de modo que pueda servir como base para futuras políticas de mitigación o educación ambiental.

#### 2. Objetivo: 

El objetivo del proyecto es analizar la evolución y el impacto de distintos contaminantes atmosféricos con la información obtenida a través de los dispositivos del SINCA en el sector sur-oriente de Santiago, comparando sus niveles, tendencias y relaciones, para poder identificar patrones relevantes y estimar un posible riesgo de salud en los habitantes del sector, por lo que la pregunta a responder es ¿Cómo afectan estos contaminantes atmosféricos a la salud de los habitantes del sector? A través de este proyecto nos gustaría concientizar a la gente de los peligros que puede ocasionar de no disminuir la contaminación ambiental a su salud, por último, nuestra audiencia objetivo son la ciudadanía en general, autoridades ambientales, instituciones educativas y de salud, especialmente aquellas relacionadas con el monitoreo y gestión de la calidad del aire.


#### Preguntas de Investigación: 

¿Cómo se comparan los niveles de monóxido de carbono (CO) en el sector con los de otros contaminantes atmosféricos?

¿Existen tendencias de mejora o deterioro en los niveles de material particulado fino (PM2,5) en los últimos años?

¿Qué relación existe entre los niveles de ozono (O3) y los de óxidos de nitrógeno (NOX) en el sector?

¿Es posible construir un modelo de predicción de los niveles de PM2,5 a partir de variables como día de la semana, hora del día y concentración de otros contaminantes?

¿Qué contaminantes presentan mayor riesgo sanitario según su frecuencia de superación de las normas de calidad ambiental en Chile?


#### 3. Diseño tentativo: 

**Organización de los datos:** revisión de las fuentes, carga de archivos y verificación de formatos.

**Limpieza de datos:** manejo de valores nulos, duplicados y detección de posibles outliers.

**Análisis exploratorio:** descripción estadística, correlaciones entre contaminantes y comparación temporal.

**Visualización:** gráficos de tendencias, mapas de calor y representaciones comparativas usando herramientas como Pandas, Matplotlib y Plotly.

**Modelado predictivo:** construcción de un modelo para predecir PM2,5 usando variables como día de la semana, hora del día y otros contaminantes.

**Conclusiones:** interpretación de resultados, vinculación con riesgos de salud y recomendaciones.

