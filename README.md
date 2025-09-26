# -IA-1-API-Data-Mashup

Project Description
This Django file serves as a food and nutrition search engine. Users may enter the name of a food, and then the application will provide:
	1. All the foods in the MealDB API that match the query
	2. while displaying the nutritional information related to the food

APIs Used
1. The MealDB API
	- Link: https://www.themealdb.com/api.php 
	- This API provides info on food, its preparatory instructions, and image references.
2. USDA FoodData Central API
	- Link: https://fdc.nal.usda.gov/api-guide
	- This API provides nutritional information on the ingredients used for the foods featured in the MealDL API

How are they used?
	- A variable like “query = 'something'”
	- is put via a format like “f’https://www.themealdb.com/api/json/v1/search.php?s{query}’
	- This will then return a list or lists of matches

How are they joined?
	- The application collects data via these APIs through queries, which are possible as the APIs are listed as lists. 
	- The APIs return a list of data that matches the query
	- These joins work as both APIs use lists to return the data, which makes it easily iterable

Limitations
	- While these APIs are incredibly useful, they are not free and have low request limits; thus, I am not entirely sure if my code works for the Nutrition API.

AI Usage Note:
	- ChatGPT was primarily used for guidance in the coding of the views section, which required the embedding of APIs and portions of the HTML/CSS, which required assistance with the formatting. 
