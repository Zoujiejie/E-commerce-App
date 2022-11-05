# E-commerce-App

## Websites
- GitHub Repo: https://github.com/Zoujiejie/E-commerce-App 
- Demo Video: https://drive.google.com/file/d/1yBmO1rCArGoSVU_HYC42Rc4aZeJFmUUH/view 

## User Story
```md
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies
```

## Acceptance Criteria
```md
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter the schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started, and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database
```

## Associations
- `Product` belongs to `Category`, as a category can have multiple products but a product can only belong to one category
- `Category` has many Product models
- `Product` belongs to many `Tag` models. Using the `ProductTag` through model, allow products to have multiple tags and tags to have many products
- `Tag` belongs to many `Product` models

