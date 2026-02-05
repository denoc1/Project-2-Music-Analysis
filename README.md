# Project-2-Music-Analysis
# 🎵 Music Streaming Data Analysis Project

## Overview
In this project, you will analyze real-world music streaming data using Java, arrays, and file input.  
You will read data from a CSV file, create objects to represent songs, and write methods that compute useful statistics about the data.

## Requirements
**This project needs to be done on your own.  You are not to use AI, CoPilot or any other AI service.**

**Comments are required for this project - but be sure they are your own, personally written, comments**
- description
- preconditions (parameter requirements)
- postconditions (return values/objects requirements)

## 📂 Data File

You will be given a file named `music_data.csv`.

Each row represents **one song**.

---

## 🧱 Part 1: Create the Song Class

Create a class named `Song`. Each `Song` object represents **one row** from the CSV file.

### Required Instance Variables

The `Song` class must include exactly the following instance variables:

- `String title`
- `String artist`
- `String genre`
- `int releaseYear`
- `double streamsMillions`
- `int durationSec`

### Required Methods

Your `Song` class must include:

- A constructor that accepts all instance variables
- Getter methods for each instance variable
- A `toString()` method that returns a readable description of a song

### Constraints

- Numeric values (streams and duration) must not be stored as Strings
- Do not add or remove instance variables
- Each object must represent exactly one song

---

## 📄 Part 2: Reading the CSV File

You will write code to read the data from `music_data.csv`.

### Required Steps

1. Create a `File` object for `music_data.csv`
2. Use a `Scanner` to read from the file
3. Skip the header line
4. Read the file line by line
5. Use `.split(",")` to separate each line into fields
6. Create a `Song` object from each line
7. Store each `Song` object in an array

### Storage Rules

- Use a fixed-size array to store the songs (you may assume there are less than 100 items in the file)
- Track how many songs are loaded using a counter variable

## 📊 Part 3: Analysis Methods

In the Project Class, create the static methods that will interact with the array of songs.

### Class Rules

- All method headers must be identical to the headers below.
- **Methods must return values or objects, not print results**
- Each method must take a `Song[]` array and a size parameter

### Required Methods

    public static Song getMostStreamed(Song[] list, int size)
    public static double getAverageStreamsByGenre(Song[] list, int size, String genre)
    public static int countSongsByDecade(Song[] list, int size, int decade)
    public static Song getLongestSong(Song[] list, int size)
    public static double getAverageDuration(Song[] list, int size)

---

## 🖥️ Part 4: Program Output

Your `main` method must:

- Load the data from the CSV file
- Print the total number of songs
- Print the most streamed song
- Print average streams for at least three different genres
- Print the number of songs released in each decade
- Print the longest song
- Print the average song duration

### Output Expectations

- Output must be clearly labeled
- Output must be easy to read

---

## ⭐ Optional Extensions (Extra Credit)

You may complete any of the following:

- Identify and print the top 3 most streamed songs
- Determine which genre has the highest average streams

---

## 📌 Final Notes

- Use meaningful variable names
- Follow proper Java formatting and indentation
- Comment your code where appropriate - not just method comments, but descriptive, in-line comments
- Ensure your program runs without errors before submitting

Good luck, and enjoy exploring the data!
