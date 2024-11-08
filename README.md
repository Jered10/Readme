# Song Lyrics Search Engine

## Overview

This project analyzes song lyrics data from a TSV file by utilizing a custom `MySearchEngine` class to perform text-based search operations. The main goal of this program is to provide an efficient search mechanism based on song lyrics, allowing users to query for relevant songs by matching terms found in the lyrics.

## Purpose

The purpose of this code is to read song lyrics data, store it in a structure optimized for fast search, and allow users to search for songs based on query terms. The search engine uses the term frequency (TF) and inverse document frequency (IDF) to calculate relevance scores for each song, enabling accurate results for text-based queries.

## Features

- **Song Lyrics Data**: Read and store song details, including title, artist, year, views, and lyrics.
- **Search Engine**: Implement a custom search engine that calculates the relevance of songs based on the query terms and their lyrics.
- **Query Matching**: Search for songs based on lyrics matching input queries and rank them according to their relevance.
- **TF-IDF Calculation**: Use TF-IDF (Term Frequency-Inverse Document Frequency) to evaluate the importance of terms within songs' lyrics.

## Components

### 1. Song Class

The `Song` class represents a song with attributes such as title, artist, year, view count, and lyrics. It also includes methods for accessing and manipulating these properties.

### 2. MySearchEngine Class

- **processAllSongs(ArrayList<Song> songs)**: This method processes all songs to calculate term frequencies (TF) for each song and the inverse document frequency (IDF) across the entire collection.
- **search(String query)**: This method allows users to search for songs using query terms. It calculates a relevance score for each song and outputs the top matches.
- **calculateRelevance(Song song, String[] query)**: This method computes the relevance score of a song based on the query terms using a custom formula that combines term frequency and inverse document frequency.

### 3. Program6 Class (Main Class)

- **main(String[] args)**: The main method reads the song lyrics data from a TSV file, initializes the search engine, and tests it with a set of queries. It outputs the results of the search, including song titles, artists, and relevance scores.

## Usage

1. **Prepare Song Data**: Ensure you have a `song_lyrics.tsv` file containing song lyrics data in the appropriate format (columns: title, artist, year, views, lyrics).
2. **Run the Program**: Execute the `Program6` class. It will read the TSV file, initialize the `MySearchEngine`, and run the search for multiple test queries.
3. **Querying**: After running the program, you can modify the queries in the code or prompt the user to input new search terms. The search engine will display the most relevant songs based on the lyrics.

## Example Output

- **Total songs loaded**: Displays the number of songs successfully loaded from the TSV file.
- **Search results**: For each query, the program outputs the top 5 songs ranked by relevance, along with the song title, artist, and relevance score.

## Author: Jered Kalombo  
## Version: 1.0
