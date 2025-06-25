# Database-of-AgriMart
One-stop-Shop for all

# AgriMart Database System

This project implements a relational database system for AgriMart using PostgreSQL. It is designed to support agricultural trade by enabling direct transactions between farmers, buyers, dealers, and transport providers. The goal is to reduce dependency on intermediaries and ensure fair pricing and efficient logistics.

## Project Overview

AgriMart serves as a backend data system for managing crop and item listings, user information, order processing, and delivery tracking. It supports both farmer-to-buyer and dealer-to-farmer transaction flows, while integrating transport services into the system.

## Technologies Used

- PostgreSQL
- Dia (for ER and relational diagrams)
- SQL (for queries and data manipulation)

## Features

- Farmers and dealers can list available crops or items with detailed information such as quantity, rate, and location.
- Buyers can place orders, view seller details, and receive deliveries through assigned transport providers.
- Transaction data includes delivery dates, ratings, freight charges, and quantities bought.
- Ratings are collected for both dealers and transport providers to maintain quality.
- Various SQL queries are written to retrieve useful insights from the data.

## Database Design

- **ER Diagram** models entities like User, Crop, Item, Address, and Transaction.
- **Relational Schema** is fully normalized to BCNF to maintain data consistency.
- Primary keys and composite keys are used appropriately across tables.
- Functional Dependencies are documented and proven for each relation.

## SQL Query Highlights

The SQL queries cover a range of use cases, including:
- Listing crops by farmer region
- Calculating total transaction amount between specific users
- Finding average transport provider ratings
- Identifying late or pending deliveries
- Ranking farmers by total revenue or ratings
- Listing items on sale or comparing prices
- Tracking crop sales by quantity or cost across different users

## Reference Files

Please refer to the following files for detailed implementation:

- `Project_Report.pdf` – Contains schema documentation, BCNF proofs, and entity definitions
- `SQL_Queries.txt` – Includes all major SQL queries for analysis and reporting
- `Relation_Schema` – Outlines all tables, attributes, and keys used in the system
- `ER_Diagram` – Visual ER representation of the entire database design
