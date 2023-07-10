# nosql_challenge
Background
--------
The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. A food magazine needs to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.
### Part 1: Database and Jupyter Notebook Set Up ###
#### Objective ####
- Import the data provided in the `establishments.json` file from the Terminal. Name the database `uk_food` and the collection `establishments`. The text for this code can be found in the first markdown cell in the `NoSQL_setup.ipynb`.
- import the libraries needed: PyMongo and Pretty Print (`pprint`).
- Create an instance of the Mongo Client.
- Confirm the database was created and that the data loaded properly by:
  - List the databases in MongoDB. Confirm that `uk_food` is listed.
  - List the collection(s) in the database to ensure that `establishments` is there.
  - Find and display one document in the `establishments` collection using `find_one` and display with `pprint`.
- Assign the `establishments` collection to a variable to prepare the collection for use.

### Part 2: Update the Database ###
#### Objective ####

Make the following changes to the establishments collection:
- Add a new restaraunt dictionary to the database.
- Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the `BusinessTypeID` and `BusinessType` fields.
- Update the new restaurant with the `BusinessTypeID` found from the step above.
- Check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.
- Some of the number values are stored as strings, when they should be stored as numbers. Change this by:
  - Using `update_many` to convert `latitude` and `longitude` to decimal numbers.
  - Using `update_many` to convert `RatingValue` to integer numbers.
### Part 3: Exploratory Analysis ###
#### Objective ####
The analysis portion of this script can be found in `NoSQL_analysis.ipynb`
To answer the proceeding questions, do the following:
- Use `count_documents` to display the number of documents contained in the result.
- Display the first document in the results using `pprint`.
- Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.
Note: The scores for Hygiene, Structural, and ConfidenceInManagement work in reverse. This means, the higher the value, the worse the establishment is in these areas.
1. Which establishments have a hygiene score equal to 20?
2. Which establishments in London have a `RatingValue` greater than or equal to 4?
3. What are the top 5 establishments with a `RatingValue` of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
<img width="218" alt="Screenshot 2023-07-10 at 12 29 04 PM" src="https://github.com/m-janssens-boop/nosql_challenge/assets/127706155/9e9bad64-0e83-477e-b8fb-c525813cce16">
