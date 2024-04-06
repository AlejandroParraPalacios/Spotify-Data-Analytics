# **UNIVERSIDAD AUTONOMA DE OCCIDENTE**
## **Especialización en Analítica de Big Data**
### **Módulo: Gestión y Almacenamiento de Datos**
### **Proyecto de Extracción, Transformación y Cargue de Datos para Análisis**
### **<font>Autores:**
- **Sergio Masso Giiraldo**
- **Daniel Otero Erazo**
- **Alejandro Parra Palacios**
</font>

## Problematica (Limitada Diversidad en Recomendaciones Musicales Personalizadas)
---
 La diversidad musical en las recomendaciones personalizadas de plataformas de streaming como Spotify se ve comprometida por la falta de apoyo institucional y la concentración en géneros populares. Esta situación limita la visibilidad de artistas emergentes y géneros menos comerciales, resultando en una oferta musical que no refleja la rica variedad de expresiones culturales.

Explicación:

- **Falta de Apoyo Institucional:** Sin un respaldo adecuado, los artistas y géneros menos conocidos luchan por obtener reconocimiento.
Concentración en Géneros Populares: Los algoritmos tienden a favorecer lo que es popular, lo que puede sesgar las recomendaciones y limitar la exploración musical.
Impacto:

- **Para los Usuarios:** Se reduce la oportunidad de descubrir música nueva y variada que podría alinearse con sus preferencias personales.
Para los Artistas: Los emergentes y los géneros menos comerciales enfrentan obstáculos para alcanzar su público, ya que las recomendaciones tienden a omitir su música.

## Contenido del reporsitorio
---
Este reporsitorio cuenta cuanta con los siguientes archivos:
- **PROYECTO_ETL.ipynb:** Notebook de Jupyter que ejecuta código Python para llevar a cabo el proceso ETL (Extracción, Transformación y Carga) desde la API de Spotify hasta una base de datos MySQL.
- **Dashboard_Spotify.pbix:** Dashboard interactivo creado a partir de los datos de MySQL, que presenta de manera dinámica y visual la información procesada, reflejando las tendencias y patrones de consumo musical.
- **Tablas.sql:** Son las utilizadas dentro de la gestión y conexión para la base de datos.

## Muestra del Dashboard
---
![image](https://github.com/AlejandroParraPalacios/Spotify-Data-Analytics/assets/129110617/b3361aa6-9acb-42f6-acd7-6bf961973889)

## Estrcutra de los datos
---
En el proceso de análisis y organización de los datos extraídos relacionados con música, hemos procedido a clasificar esta información en tres tablas principales, cada una diseñada para almacenar un conjunto específico de datos y facilitar su acceso y análisis posterior. A continuación, se detalla la estructura y el propósito de cada tabla:

- **Tabla de Tracks (Pistas):** Esta tabla constituye el núcleo de nuestra base de datos, ya que en ella se almacenan los detalles fundamentales de cada canción. La información incluida abarca el nombre de la canción, un identificador único o Primary Key (clave primaria) que facilita la interacción y relación con las otras tablas, y el nivel de popularidad de cada pista. Este último dato ofrece una visión cuantitativa del éxito o aceptación de la canción entre el público. El diseño de esta tabla permite una rápida recuperación de datos esenciales sobre las pistas musicales y sirve como punto de enlace para relacionar canciones específicas con sus respectivos artistas y características musicales.

- **Tabla de Artistas:** La función principal de esta tabla es compilar la información relacionada con los artistas o intérpretes de las canciones. Los datos recogidos aquí incluyen el nombre del artista, el número de seguidores, que proporciona una medida de su popularidad y base de fans, y el grado de popularidad del artista, que refleja su reconocimiento y éxito en la industria musical. Al almacenar estos datos, la tabla de Artistas no solo ofrece un perfil detallado de cada intérprete sino que también permite analizar tendencias en la popularidad de los artistas y su impacto en la industria.

- **Tabla de Tracks_Variables (Variables de las Pistas):** Esta tabla está dedicada a documentar las características intrínsecas de las canciones, abarcando aspectos como la danzabilidad, el nivel de acústica, la emotividad, entre otros. Al evaluar estas dimensiones, la tabla proporciona una perspectiva rica y detallada sobre la naturaleza de cada pista, permitiendo a los analistas entender mejor qué hace única a una canción y cómo estos atributos influyen en la percepción y aceptación del público. La inclusión de estas variables abre caminos para análisis más profundos sobre la música, como la relación entre la estructura de una canción y su popularidad.

## Conclusiones
---
Spotify y similares tienen el potencial de enriquecer sus recomendaciones musicales ampliando la variedad de géneros ofrecidos. Esto implica no solo considerar las preferencias individuales de los usuarios sino también integrar una mayor diversidad musical en sus sugerencias. La clave para lograr esta expansión radica en el uso de datos globales sobre tendencias musicales y en la promoción activa de artistas emergentes junto con géneros menos mainstream. Mejorar los algoritmos de recomendación para abrazar esta diversidad abordaría el problema actual de la homogeneidad en las listas de reproducción personalizadas, fomentando un apoyo más amplio a la variedad musical.
