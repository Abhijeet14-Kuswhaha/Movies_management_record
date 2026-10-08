# Movie Management System Using MongoDB

## Overview

The Movie Management System is a NoSQL database project that demonstrates how MongoDB can be used to efficiently store, manage, and analyze movie data. This project showcases practical NoSQL operations, making it easy to add, search, update, and sort movie records based on various parameters like genre, rating, release year, and director.

## Project Details

* Database Name: movieDB

* Collection Name: Movies

* Dataset: 50 structured JSON records containing popular movies across different languages and genres.

## Data Structure

Each document in the Movies collection follows this JSON schema:

{
  "movie_id": 1,
  "title": "Inception",
  "genre": "Sci-Fi",
  "year": 2010,
  "rating": 8.8,
  "language": "English",
  "duration": 148,
  "director": "Christopher Nolan"
}


## MongoDB Operations Implemented

This project covers a wide range of basic to advanced MongoDB queries:

### 1. Database & Collection Management:

Creating the database (use movieDB)

Creating the collection (db.createCollection("Movies"))

### 2. CRUD Operations:

Insert: Bulk insertion of 50 records using insertMany().

Read: Displaying records using the find() method.

Update: Modifying a specific movie's rating using updateOne() and the $set operator.

### 3. Advanced Querying & Filtering:

* Projection: Displaying only specific fields (e.g., fetching only movie titles).

* Exact Match: Filtering by attributes like language:"Hindi" or genre:"Action".

* Comparison Operators: Using $gt, $gte, and $lte to find movies released after a certain year, or within a specific duration/rating range.

* Multiple Conditions (AND): Finding movies that match multiple criteria simultaneously (e.g., Hindi AND Action).

* Logical Operators (OR): Using $or to fetch movies that belong to one genre OR another (e.g., Action OR Comedy).

### 4. Sorting and Aggregation:

* Sorting: Organizing results by rating in Ascending (1) and Descending (-1) order using sort().

* Limiting Results: Fetching the "Top 5 Rated Movies" by chaining .sort() and .limit(5).

## How to Run This Project

1. Install MongoDB and MongoDB Compass (or use the Mongo Shell / mongosh).

2. Open your Mongo terminal or Compass mongosh interface.

3. Switch to the database: use movieDB

4. Run the insertion script provided in movies.json using db.movies.insertMany([...]).

5. Execute the various find(), sort(), and updateOne() queries to explore the dataset.

## Conclusion

This project serves as a foundational guide to understanding core MongoDB concepts, including documents, collections, projection, logical querying, sorting, and data updating. It highlights the flexibility of NoSQL databases in handling real-world datasets efficiently.
