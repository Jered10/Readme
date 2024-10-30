# Song Lyrics Data Analysis

## Overview

This project analyzes song lyrics data across six genres (rap, R&B, pop, rock, miscellaneous, and country) using a custom `BinarySearchTree` class to manage `Song` objects. The primary goal is to efficiently filter and analyze song data based on various criteria, such as view counts and popular artists.

## Purpose

The main purpose of this code is to read song lyrics data from a TSV file, store it in a binary search tree, and allow for easy iteration and filtering of songs that meet specific criteria. This setup is particularly useful for identifying trends in different music genres over time.

## Features

- **Song Management**: Store song details, including title, artist, year, views, and lyrics.
- **Binary Search Tree**: Implement a `BinarySearchTree` class to manage `Song` objects efficiently.
- **Iterator Support**: Provide an iterator to filter songs based on view count and identify popular artists.

## Components

### 1. Song Class

The `Song` class represents an individual song with attributes such as title, artist, year, view count, and lyrics. It includes methods to access these properties.

### 2. BinarySearchTree Class

- **insert(Song newSong)**: This method adds a new song to the binary search tree based on its view count.
- **searchByViewCount(int minViews)**: This method retrieves songs with view counts above a specified threshold.
- **isValidBST()**: This method checks if the tree maintains the properties of a binary search tree.
- **toSortedList()**: This method converts the tree into a sorted list of songs based on view count.
- **clone()**: This method creates a clone of the binary search tree.
- **findPopularArtists()**: This method identifies artists with the most popular songs based on view counts.
- **filterSongsByViewRange(int minViews, int maxViews)**: This method filters songs within a specified view count range.

### 3. Main Class

- **runAnalysis()**: Executes the analysis by reading the TSV file, populating the binary search tree, and printing the results, including total songs processed, popular artists, and filtered songs.

## Usage

1. **Prepare Song Data**: Ensure you have a `song_lyrics.tsv` file containing the song lyrics data in the appropriate format.
2. **Run the Program**: Execute the main method in the `Main` class. It will read the TSV file, populate the `BinarySearchTree`, and output the results, including popular artists and filtered songs based on view counts.

## Author: Jered Kalombo  
## Version: 1.0
