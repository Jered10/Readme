# AVL Tree Song Manager

## Overview

This project provides a robust system for managing and searching song data using an AVL Tree structure. By implementing an automatically balanced binary search tree (BST), the AVL Tree ensures efficient insertion, deletion, and search operations, even with large datasets. The tree balances itself using rotations to maintain optimal height, allowing for faster search times compared to an unbalanced BST.

## Purpose

The purpose of this code is to enable efficient storage and retrieval of songs, particularly for scenarios where search operations need to consider high view counts. The AVL Tree balances itself after each insertion, keeping search times efficient. Users can query the tree for songs based on their view count, returning a list of popular songs that meet the specified criteria.

## Features

- **AVL Tree Structure**: Automatically balanced binary search tree with efficient insertion, search, and rotation operations.
- **Song Search by View Count**: Retrieve songs that meet or exceed a specified view count threshold.
- **Rotation Tracking**: Keep count of different rotations (left, right, left-right, and right-left) used to maintain tree balance.
- **Tree Height Calculation**: Compute and retrieve the height of the AVL Tree for performance insights.

## Components

### 1. `Song` Class

The `Song` class represents a song with attributes like title, artist, view count, and lyrics. Each song is comparable, allowing insertion into the AVL Tree based on customizable criteria.

### 2. `AVLTree` Class (extends `BinarySearchTree`)

- **Rotation Counters**: Tracks counts for left, right, left-right, and right-left rotations, helping monitor the balancing process.
- **Automatic Rebalancing**: Ensures balanced structure through rotations after each insertion.
- **Height Calculation**: Updates and retrieves node heights to assess tree balance.
- **Search by View Count**: Finds and returns songs with view counts greater than or equal to a specified threshold, traversing nodes efficiently.

### Key Methods in `AVLTree`

- **`insert(Song song)`**: Inserts a song into the AVL Tree, performing rotations to maintain balance as needed.
- **`search(int views)`**: Returns a list of songs with views greater than or equal to a specified value.
- **`getHeight()`**: Retrieves the height of the tree for performance insights.
- **Rotation Methods**:
  - **`leftRotation(Node node)`**
  - **`rightRotation(Node node)`**
  - **`getLeftRotations()`**: Returns the count of left rotations.
  - **`getRightRotations()`**: Returns the count of right rotations.

## Usage

1. **Prepare Song Data**: Create `Song` objects containing details like title, artist, view count, and lyrics.
2. **Initialize AVLTree**: Instantiate an `AVLTree` object and insert songs as needed.
3. **Search by Views**: Use the `search(int views)` method to retrieve songs that meet a minimum view count threshold.
4. **Check Rotations and Height**: Access rotation counts and tree height for insights into tree balancing.

## Example Output

- **Tree Height**: Displays the height of the AVL Tree.
- **Rotation Counts**: Shows the number of each type of rotation performed to keep the tree balanced.
- **Search Results**: Outputs a list of songs with view counts greater than or equal to the specified threshold.

## Author: Jered Kalombo  
## Version: 1.0
