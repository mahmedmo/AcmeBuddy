# 🎥 AcmeBuddy

A full-stack movie ticket booking application built with Spring Boot, MySQL, and React TypeScript. This project demonstrates clean architecture, user-friendly design, and secure authentication flows.

## Overview

AcmeBuddy provides a complete movie booking experience:
- Browse theatres and movie showtimes
- Select seats with real-time availability
- Secure user authentication and registration
- Order confirmation and ticket details

The app features a responsive UI built with React and TypeScript, backed by a Spring Boot REST API connected to MySQL for data persistence.

## Features

**Theatre & Movie Selection**  
Users can browse available theatres and view movie catalogs. Registered users get access to early screenings (highlighted in the UI).

**Interactive Seat Booking**  
The seat selection interface shows real-time availability with color-coded seats:
- Red: Unavailable
- Green: Selected
- Grey: Available

Users can choose seat types (Adult/Child) before proceeding to checkout.

**Order Confirmation**  
After booking, users receive a clean summary with ticket numbers, seats, and pricing.

## Tech Stack

**Backend**
- Spring Boot (Java 17)
- MySQL
- Maven
- BCrypt for password hashing

**Frontend**
- React with TypeScript
- Tailwind CSS
- NPM

## Running the Application

**Prerequisites**
- Java 17
- Maven
- Node.js and NPM
- MySQL

**Database Setup**
1. Execute the initialization SQL:
   ```sql
   source acmebuddy_initialization.sql;
   ```
2. Ensure MySQL is running and accessible

**Backend**
```bash
cd backend
mvn clean install
java -jar target/backend-0.0.1-SNAPSHOT.jar
```
Backend runs at `http://localhost:8080`

**Frontend**
```bash
cd frontend
npm install
npm start
```
Frontend runs at `http://localhost:3000`

## Application Screenshots

### Landing & Selection Flow

<table>
  <tr>
    <td width="50%">
      <h4>Landing Page</h4>
      <img src="./previews/landing-page.png" alt="Landing Page" />
      <p><i>Cinematic welcome screen with quick navigation</i></p>
    </td>
    <td width="50%">
      <h4>Theatre Selection</h4>
      <img src="./previews/theatre-selection.png" alt="Theatre Selection" />
      <p><i>Browse available theatres by location</i></p>
    </td>
  </tr>
</table>

### Booking Experience

<table>
  <tr>
    <td width="50%">
      <h4>Movie Catalog</h4>
      <img src="./previews/browse-movies.png" alt="Browse Movies" />
      <p><i>Browse movies with early access highlights for registered users</i></p>
    </td>
    <td width="50%">
      <h4>Seat Selection</h4>
      <img src="./previews/seat-selection.png" alt="Seat Selection" />
      <p><i>Interactive seat picker with real-time availability</i></p>
    </td>
  </tr>
</table>

### Checkout

<table>
  <tr>
    <td align="center">
      <h4>Order Confirmation</h4>
      <img src="./previews/order-confirmation.png" alt="Order Confirmation" width="70%" />
      <p><i>Clean summary with ticket details and pricing</i></p>
    </td>
  </tr>
</table>
