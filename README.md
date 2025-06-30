# Analyzing-Students-Mental-Health-SQL
# 🌍 Mental Health and International Students
![Portada del proyecto](https://raw.githubusercontent.com/Jhonatan-data/Analyzing-Students-Mental-Health---SQL/main/mentalhealth.jpg)


## 📘 Proyecto: ¿Estudiar en el extranjero afecta tu salud mental?

Una universidad internacional japonesa realizó una encuesta en 2018 para analizar cómo estudiar en otro país afecta la salud mental de sus estudiantes. El estudio fue publicado en 2019 y aprobado por varios comités éticos y regulatorios.

### 🧠 Hallazgos del estudio original

- Los estudiantes internacionales presentan **mayor riesgo de dificultades de salud mental** comparados con la población general.
- Dos factores clave predicen síntomas de depresión:
  - **Conectividad social**: Sentido de pertenencia a un grupo social.
  - **Estrés de aculturación**: Estrés relacionado con adaptarse a una nueva cultura.

## 🔍 Tu misión

Usa **PostgreSQL** para explorar los datos de la tabla `students` y determinar si los resultados son similares. En particular:

- ¿Los estudiantes internacionales tienen mayor riesgo de depresión?
- ¿Influye el tiempo de estadía en el país?
- ¿Qué relación hay entre la conectividad social, el estrés de aculturación y los síntomas de salud mental?

## 🧾 Descripción de datos

La tabla `students` incluye las siguientes columnas:

| Columna             | Descripción                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `student_id`        | Identificador único del estudiante                                          |
| `nationality`       | Nacionalidad del estudiante                                                 |
| `is_international`  | Indica si el estudiante es internacional (`TRUE` o `FALSE`)                 |
| `social_connectedness` | Nivel de conectividad social (escala numérica)                        |
| `acculturative_stress` | Nivel de estrés de aculturación (escala numérica)                    |
| `depression_score`  | Puntaje de síntomas de depresión (escala validada en psicología clínica)   |
| `length_of_stay`    | Tiempo que ha permanecido el estudiante en el país (en meses)              |

## 🧪 Tecnologías

- PostgreSQL
- SQL para análisis exploratorio

## 📈 Conclusiones del análisis
![Gráfico de resultados](https://raw.githubusercontent.com/Jhonatan-data/Analyzing-Students-Mental-Health---SQL/main/resultados.jpg)
A partir de la consulta SQL realizada y el análisis de los datos agrupados por tiempo de estadía (stay) para estudiantes internacionales, se obtuvieron las siguientes conclusiones:

## 🧠 Salud mental y tiempo de estadía
Síntomas depresivos (PHQ):

- Se observa una tendencia a la baja en los niveles de depresión a medida que aumenta el tiempo de permanencia en el país.

- Esto sugiere que los estudiantes podrían adaptarse mejor emocionalmente con el tiempo.

Conectividad social (SCS):

- Aunque presenta cierta variabilidad, en general tiende a aumentar ligeramente con el tiempo de estadía.

- Indica que los estudiantes pueden estar construyendo redes sociales y vínculos a medida que se integran al nuevo entorno.

Estrés de aculturación (AS):

- Los niveles de estrés cultural son más altos durante los primeros meses, especialmente entre el mes 3 y 6.

- Posteriormente, hay una disminución gradual, lo que sugiere un proceso de adaptación cultural progresivo.

## ⚠️ Limitaciones
- Algunos grupos tienen una cantidad limitada de estudiantes, lo que puede afectar la representatividad estadística de ciertos promedios.

- Para obtener conclusiones más sólidas, se recomienda:

- Ampliar la muestra

- Aplicar análisis estadísticos adicionales (como correlaciones o regresiones)
