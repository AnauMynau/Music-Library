# Music Library

## Description
The **Music Library** project is a simple Java-based application that allows users to manage a collection of songs and playlists. Users can add songs, search for songs by name, filter them by genre, remove songs, and display the playlist's content. The project implements Object-Oriented Programming (OOP) principles such as encapsulation, inheritance, and polymorphism.

This project was developed as part of two assignments:
- **Assignment 1**: Basic class structure with constructors, attributes, methods, and instance creation.
- **Assignment 2**: Extension of Assignment 1 with enhanced features like filtering, searching, sorting, and encapsulation.

## Features
- Add songs to a playlist.
- Search for songs by name.
- Filter songs by genre.
- Remove songs from the playlist.
- Sort songs by artist or genre.
- Display all songs in a playlist.
- Compare multiple objects using `equals()` and `hashCode()`.

## Technologies Used
- **Java 17**
- **Object-Oriented Programming (OOP)**
- **Encapsulation, Inheritance, Polymorphism**
- **Collections (ArrayList)**

## Installation & Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/AnauMynau/Music-Library.git
   ```
2. Open the project in **IntelliJ IDEA** or any Java IDE.
3. Ensure you have **Java 17+** installed.
4. Compile and run the `Main.java` file.

## Usage
Upon running the application, the user is presented with a menu:
```
What would you like to do?
1. Add New Song
2. Show Playlist
3. Search By Name
4. Filter By Genre
5. Remove Song by Name
6. Exit
```
Users can interact with the menu to manage their music library.

## Class Structure
### **1. Artist.java**
- Attributes: `artistName`, `startYear`, `popularity`
- Methods: Getters, Setters, `toString()`, `equals()`, `hashCode()`

### **2. Song.java**
- Inherits from `MusicItem`
- Attributes: `songName`, `artist`, `durationInSeconds`, `songGenre`
- Methods: Getters, Setters, `printDetails()`, `toString()`, `equals()`, `hashCode()`

### **3. Playlist.java**
- Attributes: `namePlaylist`, `songs (ArrayList<Song>)`
- Methods: `addSong()`, `printPlaylistDetails()`, `searchByName()`, `filterByGenre()`, `removeSongByName()`, `sortByArtist()`, `sortByGenre()`

### **4. MusicItem.java**
- Abstract class with `printDetails()` method.

### **5. SongManager.java**
- Handles user interactions like adding songs, searching, and filtering.

## Example Usage
### Creating an Artist and Song
```java
Artist artist = new Artist("Queen", 1970, 9.8);
Song song = new Song("Bohemian Rhapsody", artist, "5:55", "Rock");
System.out.println(song);
```
### Adding a Song to Playlist
```java
Playlist playlist = new Playlist("My Playlist");
playlist.addSong(song);
playlist.printPlaylistDetails();
```

## License
This project is for educational purposes and does not have a specific license.

---
**Contributor:** [AnauMynau](https://github.com/AnauMynau)

