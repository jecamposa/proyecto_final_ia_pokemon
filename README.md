# proyecto_final_ia_pokemon
Este repositorio tiene el proyecto final de inteligencia artificial. Un clasificador de pokemones legendarios.
# Introducción
En la serie de Pokémon, en toda la historia han existido más de 800 Pokémon. Estos tienen diferentes estadísticas, tipos, generaciones, entre otros que permiten clasificar a los Pokémon. Adicionalmente, existen unos tipos que son más raros y exclusivos que otros, los cuales son los Legendarios. Estos son unos tipos de Pokémon que son más fuertes, más rápidos y en general que cuentan con mejores estadísticas que los demás.

Para el proyecto final de inteligencia artificial, lo que se busca es, buscar un método de ML que permita realizar un clasificador de los Pokémon legendarios. Para hacer esto, primero se necesita obtener un dataset. En Kaggle, se encontró el siguiente dataset: https://www.kaggle.com/datasets/abcsds/pokemon, el cual contiene diferentes estadísticas y categorías que permiten trabajar para realizar el clasificador.

En el desarrollo del proyecto, se implementaron 3 diferentes métodos que permitían hacer el clasificador se midieron con las respectivas métricas, y finalmente se sacaron las conclusiones.
# Desarrollo
Para el desarrollo del proyecto, se utilizó la plataforma de Google Colaboratory, y se implementó en el lenguaje de programación Python. El código está estructurado de la siguiente manera:

Lo primero que se hace es hacer el llamado de las librerías, las que se usan son Pandas, para el tratamiento de datos, Numpy, también para el tratamiento de los datos, y finalmente Sklearn, para la implementación de los algoritmos de Machine Learning.
La siguiente parte del código está destinada al tratamiento de los datos, pues se debe hacer un preprocesamiento de datos para poder tratarlos de manera correcta.
![image](https://user-images.githubusercontent.com/103275887/204162760-cd2af8fe-5654-4779-866a-869d2a1733b7.png)

De graficar los datos se puede ver que hay columnas que sobran, como la de “#”, y hay columnas que contienen muchos NaN, correspondientes a los Pokémon que no tienen segundo tipo. Aquí se hace un procesamiento para eliminar estas columnas y los NaN.

Se tenían dos opciones, la primera reemplazar los valores de la columna 2 con los de la columna 1, sin embargo, se optó por eliminar la columna, pues llenando la columna no se ganaba nada, y quitándola se ahorraba memoria.

Ahora, se deben escoger las características para el clasificador, aquí se analiza el dataset, se pueden ver dos cosas, la primera, que hay una columna llamada total que da las estadísticas totales del Pokémon, y la segunda que hay dos tipos de ataque y de defensa, la normal y la especial, esto se puede condensar en un solo valor de ataque y defensa, entonces se agregan esas columnas.

Ahora, lo que se hizo fue graficar los Pokémon legendarios, para hacer un pequeño análisis de las estadísticas y saber con cuáles haces los clasificadores.
