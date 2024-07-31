# COM313-24B-API-project
Hotel Booking API
Description :The Hotel Booking API is a RESTful web service designed to manage hotel booking operations. It supports CRUD (Create, Read, Update, Delete) operations for hotels and bookings using an in-memory database. This API allows users to interact with hotel information and manage bookings.

Key Features: Manage hotel records (add, update, delete, retrieve).
Manage booking records (add, update, delete, retrieve).
Use Swagger UI for interactive API documentation and testing.

Prerequisites
.NET 7.0 SDK or later
Visual Studio 2022 or later (optional, but recommended for easier development)

Running the API
Clone the Repository:
git clone https://github.com/vrsgad/hotel-booking-api.git cd hotel-booking-api

Open the solution file (.sln) in Visual Studio or your preferred IDE
In the terminal or Package Manager Console in Visual Studio, run: dotnet restore
You can run the application from Visual Studio by pressing F5 or from the terminal using: dotnet run

Get All Hotels
Description: Retrieves a list of all hotels.
Response Example:
  {
    "id": 1,
    "name": "Grand Hotel",
    "location": "Paris",
    "rating": 4.5,
    "numberOfRooms": 100
  },
  {
    "id": 2,
    "name": "Ocean View",
    "location": "Miami",
    "rating": 4.0,
    "numberOfRooms": 80
  }
Get Hotel by ID
Description: Retrieves a single hotel by its ID.
Response Example:
{
  "id": 1,
  "name": "Grand Hotel",
  "location": "Paris",
  "rating": 4.5,
  "numberOfRooms": 100
}
Create a New Hotel
Description: Creates a new hotel.
Request Body Example:
{
  "name": "Luxury Inn",
  "location": "New York",
  "rating": 4.8,
  "numberOfRooms": 150
}

{
  "id": 3,
  "name": "Luxury Inn",
  "location": "New York",
  "rating": 4.8,
  "numberOfRooms": 150
}

Update an Existing Hotel
Description: Updates an existing hotel.
Request Body Example:
{
  "id": 1,
  "name": "Grand Hotel",
  "location": "Paris",
  "rating": 4.7,
  "numberOfRooms": 120
}   
Delete a Hotel
Description: Deletes a hotel by its ID.
Response: 204 No Content (indicates success, no content returned)

Get All Bookings
Description: Retrieves a list of all bookings.
Response Example:
  {
    "id": 1,
    "hotelId": 1,
    "customerName": "Anita Ebohoin",
    "checkInDate": "2024-07-01T00:00:00",
    "checkOutDate": "2024-07-03T00:00:00",
    "totalAmount": 200.00
  },
  {
    "id": 2,
    "hotelId": 2,
    "customerName": "Vincent Perry",
    "checkInDate": "2024-07-02T00:00:00",
    "checkOutDate": "2024-07-05T00:00:00",
    "totalAmount": 300.00
  }
  
 Create a New Booking
Description: Creates a new booking.
Request Body Example:
  {
  "hotelId": 1,
  "customerName": "Alice Johnson",
  "checkInDate": "2024-08-01T00:00:00",
  "checkOutDate": "2024-08-07T00:00:00",
  "totalAmount": 350.00
}

Update an Existing Booking
Description: Updates an existing booking.
Request Body Example:
{
  "id": 1,
  "hotelId": 1,
  "customerName": "Anita Ebohoin",
  "checkInDate": "2024-07-01T00:00:00",
  "checkOutDate": "2024-07-04T00:00:00",
  "totalAmount": 220.00
}




