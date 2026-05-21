# Online Voting System using MySQL and Python

A database-driven online voting system built using Python and MySQL. The project models voter registration, candidate and party management, vote recording, and result calculation using a relational database schema.

## Project Overview

This project simulates the backend structure of an online voting system. It uses MySQL to store voter, candidate, party, election, district, user, vote, and result data. Python is used to connect to the database and handle user-facing voting system operations.

The goal of this project was to understand how relational databases can support real-world systems that require structured data, validation, relationships between entities, and automated result tracking.

## Features

- Voter registration and eligibility checks
- Candidate, party, election, and district data management
- User table for voter login and active status tracking
- Vote recording with one vote per voter constraint
- Password validation before vote submission
- Automatic vote counting using a MySQL trigger
- SQL views for district-wise and party-wise vote analysis
- Queries for updating voter information and removing inactive users
- ERD included to show database relationships

## Tech Stack

- Python
- SQL / MySQL
- MySQL Connector for Python

## Database Design

The database includes the following tables:

- `Address`
- `Voter_Table`
- `Candidate_Type`
- `Election_Table`
- `Party_Table`
- `User_Type`
- `Candidate_Table`
- `User_Table`
- `Vote_Table`
- `Result`

The schema uses primary keys, foreign keys, unique constraints, and a trigger to maintain vote counts after new votes are inserted.

## Repository Structure

```text
Online-Voting-System-using-MySQL-and-Python/
│
├── Database Framework.sql      # Creates the database tables, constraints, and trigger
├── Insert Statements.sql       # Inserts sample voter, candidate, party, user, and vote data
├── Queries.sql                 # Contains analytical and maintenance SQL queries
├── Runner.py.py                # Python script for interacting with the MySQL database
├── ERD.jpg                     # Entity Relationship Diagram
└── README.md                   # Project documentation
