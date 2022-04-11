# INFLUENCERS DE INSTAGRAM - QUE TAN DETERMINANTE ES LA CANTIDAD DE SEGUIDORES?

## RESUMEN
Se realiza un analisis de los principales usuarios "influencers" de Instagram, tratando de entender
la relacion que existe entre la cantidad de seguidores y el engagement alcanzado. 

Que tan ifnluenciado esta por el pais de su audiencia y el rubro en el que se mueven?

# DATOS

Contamos con 997 observaciones unicas, las cuales se conforman de la siguiente manera:

|  | Nombre del Influencer | Cuenta de Instagram | Categoria Principal | Seguidores |  Principal Pais Audciencia | Engagement | Engagement Promedio |  |
|---:|---:|---:|---:|---:|---:|---:|---:|---|
| Descripcion | Nombre del Influencer dueno de la cuenta de Instagram. | el username de instagram | Rubro del contenido que comparte| Cantidad de Seguidores| Pais de donde son la mayoria de sus seguidores | Usuarios que interactuan con su contenido| Usuarios que interactuan con su contenido en promedio |  |
| Tipo de Dato | str | str | str | float | str | float | float |  |

# METODOLOGIA PARA EL ANALISIS
Se realizaron determinadas transformaciones para poder manipular los datos:
* Los datos numericos estaban en formato de texto, con 'M' para indicar millones y 'k' para indicar miles. Ambos fueron removidos y el valor multiplicado por 1e3 o 1e6 segun correspondiera.
* En los casos que solo se tenia en nombre de la cuenta de instagram y no el nombre del usuario, se uso el nombre de la misma como si fuera el nombre de pila del mismo.
* Se opto por eliminar la columna de con informacion de una segunda categoria de contendio, por tener muy pocos datos y porque no aportaba mayor valor a nuestro analisis. 
* Se creo la columna calculada "Porcentaje Engaged" para ver la relacion entre los seguidores del usuario y el engagement de los mismos.
* Se agruparon los datos segun distintas variables para evaluar el comportamiento de las mismas.


# Resultados
## Top influencers

En primer lugar vemos los Top 5 Influencers segun la cantidad de seguidores que tienen.

|   | cuenta_instagram   | nombre_del_influencer   | categoria_principal   |   seguidores | pais_audiencia   |   engagement |   engagement_promedio |   porcentaje_engaged |  |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|---|
| 1 | instagram   | Instagram     | Photography     |    4.872e+08 | India     | 352300       |         467400        |             0.095936 |  |
| 2 | cristiano          | Cristiano Ronaldo       | Sports with a ball    |    4.196e+08 | India            |      5.7e+06 |              7e+06    |             1.66826  |  |
| 3 | kyliejenner        | Kylie 🤍                | Fashion               |    3.233e+08 | United States    |      7.6e+06 |              1.23e+07 |             3.80452  |  |
| 4 | leomessi           | Leo Messi               | Sports with a ball    |    3.154e+08 | Argentina        |      4e+06   |              5.3e+06  |             1.68041  |  |
| 5 | selenagomez        | Selena Gomez            | Music                 |    3.082e+08 | United States    |      3.3e+06 |              4.4e+06  |             1.42764  |

Como podemos observar dentro de los usuarios con mas seguidores, la mayor audiencia es en dos casos Estados Unidos, en dos India y una Argentina. 
En cuanto a las categorias del contenido se repite dos veces deportes y despues figuran musica, fotografia y moda.

## Resultados
 **Graficas de la cantidad de seguidores y engament por seguidor promedio segun el Pais de Audiencia**

![]('Documents/GitHub/intro-al-analisis-de-datos/grafica_paises.png')

**Graficas de la cantidad de seguidores y engament por seguidor promedio segun la Categoria de contenido**

![](http://localhost:8888/doc/tree/Documents/GitHub/intro-al-analisis-de-datos/grafica_categorias.png)

En ambos casos, lo primero que se puede ver es la disociacion entre la cantidad de seguidores y el engagement. 
Por que es esto importante? A la hora de elegir un influencer para pagar publicidad se suele optar por la opcion con mayor canitdad de seguidores. 

La categoria con mayor cantidad de seguidores promedio es fotografia mientras que la que tiene mayor engagement por 
seguidor es Management & Marketing. 

Por lo que, considerando que los influencers suelen cobrar mas en los casos que tienen mas seguidores, seguramente segun se obtenga un mejor resultado en la inversion de quien busque una cuenta con contenido del segundo tipo.

 
