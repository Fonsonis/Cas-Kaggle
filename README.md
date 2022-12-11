## Caso Kaggle APC - [UAB: 2022-2023]

Nombre: Daniel Gutierrez Rodríguez

Dataset: [Video Games Sales 2019](https://www.kaggle.com/ashaheedq/video-games-sales-2019)

# Caso Kaggle
En esta practica analizaremos un dataset con datos sobre las ventas de los videojueos a lo largo del año 2019 (https://www.kaggle.com/ashaheedq/video-games-sales-2019). Se analizan los datos y sus valores. Se ha realizado una  normalización de los mismos y hemos trabajado con ellos mediante el uso de modelos de classificación. 

Como se explica en el informe, los datos de nuestro dataset están poco correlacionados por lo que realizar su estudio es algo complejo.

# Trabajo realizado
Con el fin de analizar nuestro dataset como se ha comentado en la parte superior, hemos debido realizar un tratamiento de los datos, normalización de los mismo y ejecución de diferentes modelos de classificación.
En un primer inicio hemos analizado las variables que contiene el dataset y sus valores. Hemos tenido que eliminar algunas de las variables debido a la gran cantidad de nulls que estas variables contenian. Hemos hecho esto puesto que normalizar una cantidad ingente de nulls puede causar una alteración de los datos reales y que nos lleve a valores erròneos alejados de la realidad. 
Posteriormente hemos eliminado los NaN y la variable Status puesto que tras lanzar una primera ejecución de la matriz de correlación hemos visto que era un valor constate sin ningún tipo de relevancia. 
Finalmente dentro de la sección de procesamiento de los datos hemos tenido que sustituir los valores de las variables que guardaban datos del tipo String. Esto es debido a que no es posible realizar una investigación de correlación entre variables de tipo numérico y variables de tipo caracter, por lo que hemos sustituido los valores tipo "String" por identificadores únicos, permitiendo así estudiar la posible correlación con otras variables. 

Una vez realizado todo este procesamiento de los datos hemos llevado a cabo tanto el entrenamiento com la validación de ese entrenamiento de nuestro dataset. Se han lanzado dos modelos de clasificación para poder ver que tipo de relación guardan las variables de nuestro dataset y hemos visto que se trata de un dataset con las variables muy poco relacionadas entre ellas. 
Pese a los bajos resultados, hemos llegado a la conclusión de que el modelo que mejor trabaja con nuestro dataset es "Decision Tree" con el hyperparámetro de "gini". 

# Conlcusiones
A lo largo de todo el informe hemos visto que los datos de nuestro dataset no guardan correlación entre ellos, por lo que la aplicación de un modelo de classificación se vuelve complicada.

Aún así, tras realizar varias pruebas hemos visto que el modelo de classificación que mejor se ajusta es el modelo de Decision Tree con una media de 0.378 de exito.

Con esto podemos concluir que nuestra hipotesis principal sobre la casi inexistente correlación de las variables del dataset, y más en concreto con el género eran correctas, y no guardan relación.
