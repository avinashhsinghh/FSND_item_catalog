# Item Catalog Project  
Developed a content management system using the Flask framework in Python. Authentication is provided via OAuth and all data is stored within a PostgreSQL database. Authenticated users will have the ability to post, edit, and delete their own items.  

## Tools and Frameworks
This web application was built with HTML5, CSS, Bootstrap, Vagrant, Flask, SQLAlchemy, Google and Facebook Oauth2 & APIs.

## Instruction
To run the web application:    
1. From directory */FSND_item_catalog*, initialize the application database by typing `python database_setup.py`  
3. From directory */FSND_item_catalog*, run the application within the VM by typing `python main.py` into the Terminal.  
3. Access the application by visiting http://localhost:8000 locally on the browser.

## Screenshot of Cover Page

<img src="assets/cover_page.png" width="800">

## JSON Endpoints

`/catalog.json` - Returns JSON of all items in catalog

<img src="assets/catalog_json.png" width="800">

`/<category_name>/items.json` - Returns JSON of for all items of a specific category.

<img src="assets/catalog-itemJSON.png" width="800">

`/categories.json` - Returns JSON of all categories in catalog

<img src="assets/categories_json.png" width="800">

## REST Endpoints

#### --------------------------------------
#### CRUD for categories
#### --------------------------------------

`/` or `/categories` - Returns catalog page with all categories and recently added items

<img src="assets/categories1.png" width="800">

<img src="assets/categories-loggedin.png" width="800">

`/categories/new` - Allows user to create new category

<img src="assets/category-new.png" width="800">

`/categories/<int:category_id>/edit/` - Allows user to edit an existing category

<img src="assets/category-edit.png" width="800">

`/categories/<int:category_id>/delete/` - Allows user to delete an existing category

<img src="assets/category-delete.png" width="800">

#### --------------------------------------
#### CRUD for category items
#### --------------------------------------

`/categories/<int:category_id>/` or `/categories/<int:category_id>/items/` - returns items in category

<img src="assets/catalog-item.png" width="800">

`/categories/<int:category_id>/item/<int:catalog_item_id>/` - returns category item

<img src="assets/catalog-item-detail.png" width="800">

`/categories/item/new` - return "This page will be for making a new catalog item

<img src="assets/catalog-item-new.png" width="800">

`/categories/<int:category_id>/item/<int:catalog_item_id>/edit` - return "This page will be for making a updating catalog item"

<img src="assets/catalog-item-edit.png" width="800">

`/categories/<int:category_id>/item/<int:catalog_item_id>/delete` - return "This page will be for deleting a catalog item"

<img src="assets/catalog-item-delete.png" width="800">

#### --------------------------------------
#### Login
#### --------------------------------------

`/login` - login page

<img src="assets/login_page.png" width="800">


## Possible improvements

- Styling and layout could improve
- Implement CSRF protection on CRUD operations.
