# Location Tracker 🌍

A web application to visually track the countries visited by each family member on a world map. Each member is assigned a unique color, and the countries they visited are highlighted in their chosen color, making it easy to distinguish and celebrate everyone's travel adventures.

---

## Features

- **Add Family Members**: Create profiles by adding names and assigning unique colors to each member.
- **Interactive World Map**: Highlight countries visited by family members in their assigned colors.
- **Manage Visits**: Add, update, or remove visited countries for each member.
- **Dynamic Visualization**: The map updates instantly to reflect changes.
- **Database Integration**: All data is stored securely in PostgreSQL for persistence.

---

## Technologies Used

### Frontend
- **HTML**: Structure for the web pages.
- **CSS**: Styling for a visually appealing UI.
- **Bootstrap**: For responsive design and prebuilt components.
- **JavaScript**: Interactive map functionality.
- **Embedded JavaScript (EJS)**: Template engine for dynamic rendering.

### Backend
- **Node.js**: Server-side JavaScript runtime environment.
- **Express.js**: Web application framework for handling routes and requests.

### Middleware
- **body-parser**: Parses incoming requests for easy access to data.

### Database
- **PostgreSQL**: Relational database for storing and managing family members and their visited countries.

---

## Database Schema

### Table 1: `countries`
| Column         | Type       | Description                      |
|----------------|------------|----------------------------------|
| `id`           | INTEGER    | Unique identifier for the country |
| `country_code` | VARCHAR(3) | ISO country code                 |

### Table 2: `visited_countries`
| Column         | Type       | Description                     |
|----------------|------------|---------------------------------|
| `user_id`      | INTEGER    | Unique identifier for the user  |
| `country_code` | VARCHAR(3) | ISO code of the visited country |

---

## CRUD Operations

- **Create**: Add new family members and visited countries.
- **Read**: View all family members and their visited countries.
- **Update**: Edit member details or update visited countries.
- **Delete**: Remove family members or delete visited countries.
- **Inner Joins**: Used to fetch and combine data from `countries` and `visited_countries` tables for efficient queries.
Set up the PostgreSQL database:

## Create the database and tables as per the schema above.
- **Update the connection details in the project.**



## Future Enhancements
- **User Authentication: Add secure login functionality for family members.**
- **Search and Filter: Allow filtering of countries by continent or date of visit.**
- **Mobile-Friendly Interface: Enhance UI for mobile devices.**
- **Advanced Visualizations: Display travel stats like the number of countries visited.**

  *P.S.: Some of the URLs in the code to locate files may need to change.*
