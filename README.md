## <h1 align=center> Proyecto Individual 02

## <h1 align=center> Modelo de Machine Learning para predicción de precios de bienes inmobiliarios en EE.UU.
  
<p align="center">
<img src=https://s3.stackabuse.com/media/guided+projects/hands-on-house-price-prediction-machine-learning-in-python-thumbnail.jpg>
  
Hola! Mi nombre es Cristian Papini y este es mi segundo proyecto individual, el cual se basa en la creación de un modelo de Machine Learning.
 
    
## Objetivo
 Este tiene como objetivo la predicción de precios de bienes inmobiliarios en los Estados Unidos teniendo en cuenta diversas características.

## Contexto
Dentro de la sociedad globalizada e industrializada, es sabido que los precios de los inmuebles han presentado un constante cambio, por lo que quienes deseen invertir o vender una propiedad se enfrentan al fenómeno especulativo existente en la valorización de éstos. Esto, debido a la constante tendencia de las ciudades a crecer demográfica y comercialmente, llegando a un punto en donde no se tiene certeza de la valorización real dentro del sector en donde se desee invertir. Pese a que el precio depende, en cierta medida, de las tendencias que esté teniendo el mercado inmobiliario en un determinado tiempo, poder estimar adecuadamente el valor de una propiedad es una referencia clave para entender si es una buena oportunidad, ya sea de compra o de venta.   

## Plan de trabajo
Se cuenta con un dataset de 346479 registros y 22 dimensiones, las mismas son:

- id: Identificador del anuncio.
- url: Link web del anuncio.
- region: Región de Estados Unidos en donde se encuentra la propiedad.
- region_url: Link web de los anuncios pertenecientes a la región.
- price: Precio de la propiedad en dólares.
- type: Tipo de propiedad.
- sqfeet: Metros cuadrados de la propiedad.
- beds: Cantidad de dormitorios.
- baths: Cantidad de baños.
- cats_allowed: Si se permiten gatos en la propiedad toma el valor 1, 0 para caso contrario.
- dogs_allowed: Si se permiten perros en la propiedad toma el valor 1, 0 para caso contrario.
- smoking_allowed: Si se permite fumar en la propiedad toma el valor 1, 0 para caso contrario.
- wheelchair_access: Si la propiedad posee acceso para sillas de ruedas toma el valor 1, 0 para caso contrario.
- electric_vehicle_charge: Si la propiedad posee cargador para vehículos eléctricos toma el valor 1, 0 para caso contrario.
- comes_furnished: Si la propiedad viene amueblada toma el valor 1, 0 para caso contrario.
- laundry_options: Opciones de lavandería (w/d in unit: Lavadora/secadora en la propiedad, w/d hookups: conexión para lavadora/secadora, laundry on site: servicio de lavandería en el lugar, laundry in bldg: servicio de lavandería en el edificio, no laundry on sit: sin servicio de lavandería).
- parking_options: Opciones de estacionamiento (off-street parking: zona de estacionamiento, attached garage: garaje incluido, carport: cochera/garaje abierto, detached garage: garaje separado, street parking: estacionamiento delimitado en la calle, no parking: sin estacionamiento, valet parking: estacionamiento con servicio valet).
- image_url: Link web de la imagen de la propiedad en el anuncio.
- description: Descripción de la propiedad puesta en el anuncio.
- lat: Latitud.
- long: Longitud.
- state: Código del estado al que pertenece la propiedad.

Con toda esta información, para simplificar el dataset, lo primero que se hizo es descartar ciertas variables debido a su poco efecto sobre el precio del inmueble. Luego se fue transformando el dataset para así lograr limpiarlo completamente, normalizarlo y así poder tenerlo listo para correr un modelo de ML. En el Notebook que se encuentra en este repositorio se explica en mayor detalle las transformaciones que se llevaron a cabo.


## Modelo de Machine Learning
Luego de haber analizado el dataset, los objetivos y las herramientas disponibles se ha decantado por la idea de basar el modelo en el metodo Random Forest Classifier. El mismo no solamente que es uno de los más reconocidos por su eficiencia y eficacia a la hora de predicciones en datasets similares con el que se cuenta en esta situación
Como se puede ver en el Notebook, la métricas de este modelo son las siguientes:
- Accuracy en entrenamiento: 99%
- Accuracy en test: 88.5%

