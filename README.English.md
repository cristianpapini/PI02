## <h1 align=center> Project 02

## <h1 align=center> Machine Learning model for US real estate price prediction.
  
<p align="center">
<img src=https://s3.stackabuse.com/media/guided+projects/hands-on-house-price-prediction-machine-learning-in-python-thumbnail.jpg>
  
Hello! My name is Cristian Papini and this is my second individual project, which is based on the creation of a Machine Learning model.
 
    
## Objective
 This project aims to predict real estate prices in the United States taking into account various characteristics.

## Context
Within the globalized and industrialized society, it is known that the prices of real estate have presented a constant change, so those who wish to invest or sell a property face the speculative phenomenon existing in the valuation of these. This is due to the constant tendency of cities to grow demographically and commercially, reaching a point where there is no certainty of the real value within the sector where you want to invest. Despite the fact that the price depends, to a certain extent, on the trends that the real estate market is having at a certain time, being able to adequately estimate the value of a property is a key reference to understand if it is a good opportunity, either for buying or selling.   

## Workplan
There is a dataset of 346479 records and 22 dimensions, they are:

- id: Ad identifier
- url: Ad web link
- region: Region of the United States where the property is located
- region_url: Web link of the ads belonging to the region
- price: Price of the property in dollars
- type: Kind of property
- sqfeet: Square meters of the property
- beds: Number of bedrooms
- baths: Number of bathrooms
- cats_allowed: If cats are allowed in the property it takes the value 1, 0 otherwise
- dogs_allowed: If dogs are allowed on the property, it takes the value 1, 0 otherwise
- smoking_allowed: If smoking is allowed in the property, it takes the value 1, 0 otherwise
- wheelchair_access: If the property has wheelchair access, it takes the value 1, 0 otherwise
- electric_vehicle_charge: If the property has a charger for electric vehicles, it takes the value 1, 0 otherwise
- comes_furnished: If the property comes furnished, it takes the value 1, 0 otherwise
- laundry_options: Laundry Options (w/d in unit: Washer/dryer on property, w/d hookups: washer/dryer hookups, laundry on site: laundry on site, laundry in bldg: laundry in building, no laundry on sit: no laundry service)
- parking_options: Parking options (off-street parking: parking zone, attached garage: garage included, carport: carport/open garage, detached garage: detached garage, street parking: delimited parking on the street, no parking: no parking, valet parking: valet parking)
- image_url: Web link of the image of the property in the ad
- description: Description of the property placed in the ad
- lat: Latitude
- long: Longitude
- state: Code of the state to which the property belongs

With all this information, to simplify the dataset, the first thing that was done was to rule out certain variables due to their little effect on the property price. Then the dataset was transformed in order to clean it completely, normalize it and thus be able to have it ready to run an ML model. The Notebook found in this repository explains in greater detail the transformations that were carried out.
  
## Machine Learning Model
After having analyzed the dataset, the objectives and the available tools, it was concluded that it would be best to base the model on the Random Forest Classifier method. This is one of the most recognized for its efficiency and effectiveness when it comes to predictions in similar datasets that are available in this situation.
As can be seen in the Notebook, the metrics of this model are the following:
- Accuracy during training: 99%
- Accuracy during test: 88.5%
