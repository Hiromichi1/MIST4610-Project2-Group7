# MIST 4610 Project 2: Movie Theater Management System

Rachel Davies, Hiromichi Kikuchi, Anirudh Pothuri, and Sakshi Sinha


## Description
This movie theater database efficiently manages theater operations, including movie scheduling, ticket sales, auditorium capacity, and customer interactions. It tracks movies, showtimes, and ticket transactions, while also organizing theater rooms and seating arrangements. Customer data is stored to track purchasing history and preferences. The database links customers, tickets, movies, and auditoriums, providing a streamlined system for managing daily box office activities. While comprehensive for operational needs, it focuses on improving efficiency and optimizing the movie-going experience.

![Movie Theater Data Model](datamodel_movietheater.png)

- **Movie:** Stores movie details, including title, genre, runtime, and content rating.
- **Showtime:** specific times when movies are screened, linking a movie to a theater room.
- **Ticket:** Transaction records linking customers to specific seats and showtimes.
- **Customer:** Contains customer information like name and email for receipts.
- **Auditorium:** Details about the physical theater rooms and their capacities.
- **Seat:** Specific seating arrangements within each auditorium.
- **Theater:** General theater facility information.
- **Worker:** Employee details for staff managing the theater.
- **Menu_Item:** Concession items available for purchase.
- **Theater_has_Menu_Item:** Tracks which concession items are available at which theater location.

## Data Dictionary

#### Workers
![Workers](Workers.png)

#### Customer
![Customer](Customer.png)

#### Movie
![Movie](Movie.png)

#### Seat
![Seat](Seat.png)

#### Showtime
![Showtime](Showtime.png)

#### Theater
![Theater](Theater.png)

#### Theater_has_Menu_Item
![Theater_has_Menu_Item](theater_has_menu_items.png)

#### Menu_Item
![Menu_Item](Menu_Items.png)

#### Ticket
![Ticket](Ticket.png)

## Queries

![Query Matrix](queries_table_with_attributes.png)

#### 1. Identify Top-Performing Movies by Revenue
Helps managers know which movies generate the most money across all theaters.

![Query1](query_1.png)

#### 2. Determine Theater Staffing Cost per Month
Allows management to assess labor expenses per theater for budgeting.

![Query2](query_2.png)

#### 3. Find Peak Showtime Hours Across All Theaters
Helps managers allocate staff and schedule popular time slots.

![Query3](query_3.png)

#### 4. Identify Customers Who Frequently Attend Movies
Useful for loyalty program targeting, targeted marketing, or upselling.

![Query4 Code](query_4.png)
![Query4 Result](query_4_results.png)

#### 5. Auditorium Utilization Rate
Helps managers understand which auditoriums are underused or overused and adjust scheduling.

![Query5 Code](query_5_.png)
![Query5 Result](query_5_results.png)

## Tableau Visualizations

![Theater Dashboard](tableau.png)

### Top Selling Movies
- **Purpose:** This chart displays a ranking of movies by the total number of tickets sold.
- **Relevance:** Helps identify the highest-grossing films currently in rotation, aiding in decisions on which movies to retain and which to drop.

### Peak Operational Hours
- **Purpose:** Shows the count of tickets sold broken down by the hour of the day.
- **Relevance:** Highlights peak operational hours, allowing management to optimize staff scheduling and reduce wait times.

### Auditorium Utilization
- **Purpose:** Compares ticket sales volume across different theater auditoriums.
- **Relevance:** Indicates which rooms are performing best, ensuring popular movies are assigned to larger auditoriums to maximize revenue capacity.
