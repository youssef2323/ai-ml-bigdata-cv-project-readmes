# Parallel Movie Ticket Booking System

This project is a multithreaded Python application for booking movie tickets, allowing multiple users to book seats concurrently. The system features a GUI for both users and administrators, ensuring real-time synchronization, thread safety, and dynamic updates.

---

## Examples of Results

### Admin Panel

![Admin Panel](./Screenshots/Screenshot_(498).png)

### User Booking Interface

![User Interface](./Screenshots/Screenshot_(496).png)
![User Interface](./Screenshots/Screenshot_(497).png)

### Multithreaded Simulation

![Multithreading](./Screenshots/Screenshot_(499).png)
![Multithreading](./Screenshots/Screenshot_(500).png)
![Multithreading](./Screenshots/Screenshot_(501).png)

---

## Functionalities

### User Features
- **Movie Selection**: Users can choose a movie and showtime from a dynamic list.
- **Seat Booking**:
  - Select a seat from the displayed seating layout.
  - Enter the username to confirm the booking.
  - Handles synchronization to prevent double-booking.
- **Real-Time Seat Status**:
  - Visual representation of available, booked, and locked seats.
  - Requires manual refresh to see changes from other threads.

### Admin Features
- **Add Movie**: Insert new movies with showtimes and initialize seating arrangements.
- **Reset Seats**: Reset all bookings and seat statuses for a specific movie.
- **View Bookings**: Display a detailed list of all bookings for a selected movie.
- **Delete Movie**: Remove a movie and all associated seat data.

### Multithreading Features
- **Concurrent Booking**: Multiple users can book seats simultaneously via threads.
- **Synchronization**: Ensures thread safety using `threading.Lock`.
- **Deadlock and Starvation Prevention**:
  - Proper lock management ensures no thread is indefinitely blocked.
- **Performance Testing**:
  - Benchmarking of single-threaded vs. multithreaded booking scenarios.

---

## Technologies Used

| Technology       | Description                                            |
|-------------------|--------------------------------------------------------|
| **Python**       | Programming language used for application logic.       |
| **Tkinter**      | GUI development for user and admin interfaces.         |
| **MySQL**        | Database for storing movies, seats, and bookings.      |
| **Threading**    | For handling multiple user actions concurrently.       |

---

## Project Features

| Feature                          | Description                                                             |
|----------------------------------|-------------------------------------------------------------------------|
| **GUI**                          | Separate threads for user actions to prevent UI hanging.                |
| **Thread Safety**                | Synchronization via locks to avoid race conditions.                     |
| **Dynamic Seat Updates**         | Reflects real-time booking changes across multiple threads.             |
| **Admin Management**             | Admin tools for managing movies and bookings.                           |
| **Multithreading Benchmarking**  | Performance comparison between single-threaded and multithreaded modes. |

