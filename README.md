# Real-Time Multiplayer Canvas Project

Welcome to the Real-Time Multiplayer Canvas Project! This project allows multiple users to connect, create records, and interact in real-time on a shared canvas, facilitated by a robust network architecture.

## Features

- **Real-time Interaction:** Users can update their positions on a shared canvas, and changes are instantly reflected for all connected users.

- **User Records:** Player data, including names and positions, is stored in a MySQL database. Players can create records and bind together in the game.

- **Network Architecture:** The game employs a server-client architecture to manage communication between connected clients, ensuring a seamless multiplayer experience.

## Prerequisites

Before running the project, make sure you have the following installed:

- Python 3
- MySQL (for server-side database)

## Getting Started

1. Clone the repository:

```
git clone https://github.com/VargaBalazsAdam/Py-Network-Architecture.git
```

2. Navigate to the project directory:
```
cd Py-Network-Architecture
```
2.1 Install requirements
```
pip install mysql-connector-python
```
3. Set up the MySQL database:
    - Create a new database named `player_data`.
    - Run the SQL create command:
```sql
CREATE TABLE players (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    x INT NOT NULL,
    y INT NOT NULL
);
```
4. Run the server:
```
python server.py
```
5. Run the client:
```
python client.py
```
6. Enter your player name when prompted, create records, and enjoy the real-time interaction facilitated by the robust network architecture!

## Gifes, images
### Real time update
![Real time update](https://github.com/VargaBalazsAdam/Py-Network-Architecture/blob/main/gif1.gif)
### Read from database
![Read from database](https://github.com/VargaBalazsAdam/Py-Network-Architecture/blob/main/gif2.gif)

## Server Details

The server manages the communication between clients, updates player positions in real-time, and stores player data in a MySQL database.

## Client Details

Clients use the Tkinter library for the graphical user interface. Players can click on the canvas to update their positions, create records, and observe the real-time actions of other connected players.

## Contributing

Feel free to contribute to the project by opening issues or submitting pull requests. Your contributions are highly appreciated!

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
