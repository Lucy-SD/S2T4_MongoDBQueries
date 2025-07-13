# 📚 MongoDB Query Exercises

**👨‍💻 Author**: Lucy Castro

**🧠 Learning Focus**: MongoDB Query Language, Aggregation, Geospatial Queries

**🛠️ Tools**: MongoDB, MongoDB Compass, JSON Data

**💾 Database**: New York Restaurants


## 📄 Description

This repository contains MongoDB query exercises focused on:

- CRUD operations with find()

- Projection and field exclusion

- Complex filtering with operators ($gt, $lt, $in, $regex)

- Array manipulation and nested document querying

- Geospatial queries and data type checks

- Sorting and pagination


## 💻 Technologies Used

🔹 MongoDB 6.0+

🔹 MongoDB Compass (GUI)

🔹 JSON/BSON data formats

🔹 Geospatial coordinate queries


## 📋 Requirements

✅ MongoDB installed (Download)

✅ MongoDB Compass (Download)

✅ restaurants.json dataset

✅ Basic NoSQL concepts


## 🛠️ Installation

Import dataset:

mongoimport --db nyc --collection restaurants --file restaurants.json

Verify in MongoDB Compass:
javascript
use nyc

db.restaurants.countDocuments() // Should return > 25k documents

## 📂 Exercise Catalog

<details> <summary><strong>🍽️ Level 1: Basic Queries (17 Queries)</strong></summary>

  Core Concepts:

Field projection ({_id: 0})

Basic filtering (borough: "Bronx")

Pagination (limit(), skip())

Sorting (sort({name: 1}))

</details><details> <summary><strong>🔍 Level 2: Intermediate Queries (8 Queries)</strong></summary>
Core Concepts:

Compound filters without $and

Array element matching (grades.1.grade: "A")

Exclusion operators ($ne, $nin)

Geospatial queries (coord.1: {$gt: 42, $lte: 52})

</details><details> <summary><strong>🚀 Level 3: Advanced Queries (5+ Queries)</strong></summary>
Core Concepts:

Type checking (coord: {$type: "double"})

Modulo operations ($mod)

Complex regex patterns (/mon/, /^Mad/)

Combined logical conditions

</details>



## 📊 Progress Tracking

Level	Requirement	Badge

🥉 1	--> 17 correct queries

🥈 2	--> 18-25 correct queries

🥇 3 -->	26+ correct queries



## 🎯 Learning Goals

✅ Master MongoDB query syntax

✅ Project fields efficiently

✅ Query nested arrays and objects

✅ Combine operators for complex filtering

✅ Implement geospatial data queries

✅ Optimize read performance


## 🏆 Best Practices Implemented

✔️ Selective Projection: Reduce network overhead

✔️ Index Utilization: Implicit use of _id index

✔️ Regex Anchors: ^ for prefix, $ for suffix

✔️ BSON Types: Native type checks ($type)

✔️ Explicit Sorting: Ensure deterministic ordering


## 🤝 Contributions

⭐ Star the repository

🍴 Fork the project

📥 Submit pull request with:

Solution code

Sample output screenshot


## 🚀 Thanks for Visiting ¡!
