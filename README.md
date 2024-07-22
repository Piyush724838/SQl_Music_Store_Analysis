# Music Store Data Analysis

This project focuses on analyzing music store data with SQL. The dataset has 11 tables: Employee, Customer, Invoice, InvoiceLine, Track, MediaType, Genre, Album, Artist, PlaylistTrack, and Playlist. This project intends to answer many questions and obtain important insights into the music store's operations by applying SQL queries to the dataset.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Questions and Answers](#questions-and-answers)
  - [Question Set 1 - Easy](#question-set-1---easy)
  - [Question Set 2 - Moderate](#question-set-2---moderate)
  - [Question Set 3 - Advanced](#question-set-3---advanced)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Contributing](#contributing)

## Introduction
The "Music Store Data Analysis" project offers a comprehensive analysis of the music store's data to facilitate better decision-making, identify trends, and understand customer behavior. By leveraging SQL queries and data exploration, this project provides valuable answers to optimize inventory management, target marketing campaigns, and make informed business decisions.

## Dataset
The dataset for this project has 11 tables: Employee, Customer, Invoice, InvoiceLine, Track, MediaType, Genre, Album, Artist, PlaylistTrack, and Playlist, as well as their associations.

### Schema
![Schema](path_to_schema_image)

## Questions and Answers

### Question Set 1 - Easy
**Q1. Who is the most senior employee based on job title?**
```sql
SELECT * FROM EMPLOYEE
ORDER BY LEVELS DESC
LIMIT 1;****

**Q2. Which countries have the most Invoices?**
```sql
SELECT BILLING_COUNTRY, COUNT(*) AS Most_Invoices 
FROM INVOICE
GROUP BY BILLING_COUNTRY
ORDER BY Most_Invoices DESC;
