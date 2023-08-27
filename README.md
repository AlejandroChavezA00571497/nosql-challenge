# nosql-challenge
Module 12 Challenge for the Tec de Monterrey Data Analysis Bootcamp, Introduction to NoSQL

Jupyter Notebbok files that connect to a MongoDB database in order to extract information, update it and analyze it.

Main_NoSQL_setup.ipynb is the first file, it uses the following command: mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json
To import the dataset into MongoDB, provided that you are located in the "Resources" directory that has the establishments.json file in it.
It starts by importing dependencies, creating an instance of MongoClient, and assigning the database and collection inside of it to variables.
Then, the collection is updated through inserting a provided dictionary structure with new data into it, finding information about the new establishment added, updating it, changing data types and using various PyMongo methods in order to learn more about the dataset.

Main_NoSQL_analysis.ipynb is the second file, it interacts with the same dataset through an instance of MongoClient, and then exploratory analysis is performed through various queries, sorting and limiting, as well as passing the information from the MongoDB collection into Pandas DataFrames. Aggregate functions are also used, with a pipeline of different stages, in order to make more complex queries, and again, storing the information from that pipeline into a Pandas DataFrame.

The main files for this project exist on the main directory, which also contains the Resources directory, where the created establishments.json file exists.

Contributions:
- Data Analysis Bootcamp Classes
- https://www.mongodb.com/docs/manual/
- https://pandas.pydata.org/docs/user_guide/dsintro.html#dataframe
