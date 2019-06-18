# Red-Neuronal
Programa para entrenar una red neuronal artificial para identificar el genero de una persona con base en el nivel de andrógeno y estrógeno. Utilizando como función de activación tanh (Tangente Hiperbólica).

<b>Funcionamiento:</b>
A continuación se presentará el funcionamiento de la aplicación en tres partes: Entendiendo la interfaz, Ejecución y Consideraciones adicionales.

<b>i. Entendiendo la Interfaz:</b>

Al correr ‘TallerNo9_DanielBeltranPenagos_MatemáticasAplicadas’ se encontrará con la siguiente interfaz de usuario:

  <img src="/docs/doc1.png" width="500px"/><br>

La tabla que se muestra exhibida corresponde a los casos dados para la definición del género, estos mismos casos se utilizarán para el entrenamiento de la red.

  <img src="/docs/doc2.png" width="500px"/><br>

El botón de entrenar corre una función que calcula los pesos ideales para la definición del género en una prueba específica. A continuación se muestran entonces dos parámetros de entrada “Andrógeno” y “Estrógeno” que son respectivamente los valores de andrógeno y estrógeno para definir el género de la persona. El botón probar define el género de la persona con los parámetros de entrada de “Andrógeno” y “Estrógeno”.

<b>ii. Ejecución:</b>

El orden de ejecución del programa trata del entrenamiento y luego de la prueba sobre un caso, entonces se hará así respectivamente. Primero en el navegador que se tenga se abrirá la consola (Para el caso de Chrome: Click derecho->Inspeccionar Elemento-> Console)

 <img src="/docs/doc3.png" width="500px"/><br>
 <img src="/docs/doc4.png" width="500px"/><br>
 
 
En la consola al paso de la ejecución de la aplicación se mostrarán las operaciones realizadas y la información de la red. Al inicio saldrá entonces la información relacionada con la red al momento: Pesos Iniciales (W1, W2, Wo), Umbral y Factor de Aprendizaje. 

Lo que se hará a continuación entonces será entrenar la red. Se da click al botón entrenar para realizar esta acción:
 
 <img src="/docs/doc5.png" width="500px"/><br>
Cuando finalice se disparará un anuncio avisando:
 
 <img src="/docs/doc6.png" width="500px"/><br>

Y en la consola se muestra la información de los cálculos de los pesos y su resultado:

  <img src="/docs/doc7.png" width="500px"/><br>
 <img src="/docs/doc8.png" width="500px"/><br>
 

Ya que se ha entrenado a la red entonces se probarán los casos “3.9 Andrógeno, 3.9 Estrógeno” que debe dar ‘Mujer’ y “3.9 Andrógeno, 1.8 Estrógeno” que debe dar ‘Hombre. Se tomaron estos dos casos para evidenciar el funcionamiento, sin embargo funciona igual para el resto de los casos definidos. Después de ingresar los datos se debe dar click en probar:

 <img src="/docs/doc9.png" width="500px"/><br>
 <img src="/docs/doc10.png" width="500px"/><br>
 
Efectivamente funciona y se pueden revisar en la tabla que esos valores si coinciden:

 
 <img src="/docs/doc11.png" width="500px"/><br>

<b>iii. Consideraciones Adicionales:</b>

-	Los pesos iniciales se tomaron como aleatorios en un rango de 0 a 5. 
-	El umbral se toma como 0.5 debido al ejemplo anexado al taller. 
-	El ejercicio se realiza con factor de aprendizaje y su valor es 0.2, se tomó este valor debido a que habitualmente se usa ese número.
-	El resultado de la función de activación es 1 si la tangente hiperbólica de la suma producto de los pesos es mayor a 0, de lo contrario es el resultado es 0.
-	La clasificación de género es 1 para Hombre y 0 Para Mujer.
-	Lo anterior se encuentra debidamente documentado en el proyecto y así mismo las fórmulas utilizadas.

