# Twitter Sentiment Analysis Program  

This project provides a robust system for analyzing Twitter data using **custom Heap and HashMap implementations**. It efficiently handles tweet data, tracks user activity, and analyzes sentiment through an intuitive, interactive interface. The system also monitors performance by displaying build times and heap operation metrics.

---

## Purpose  

The purpose of this program is to enable efficient management and analysis of tweets using custom **Heap and HashMap-based implementations**. The system processes tweet datasets, maintains chronological ordering, and provides real-time access to user activity while tracking performance metrics.  

Users can monitor system efficiency through measurements of data loading times and heap operations.

---

## Features  

- **Custom Heap Implementation:** Efficient priority-based storage of tweets by timestamp.  
- **Custom HashMap Implementation:** Maps users to their respective tweet heaps.  
- **Performance Tracking:** Detailed monitoring of build times and heap operations.  
- **User Interface:** Interactive command-line menu system.  
- **Tweet Management:** View and delete recent tweets.  
- **Error Handling:** Comprehensive exception management.  

---

## Components  

### Tweet Class  
The `Tweet` class represents tweets with content and metadata, implementing `Comparable` for chronological ordering in the heap structure.

### MyHeap Class  

- **Priority Ordering:** Maintains the most recent tweets at the root.  
- **Dynamic Resizing:** Automatically adjusts size for optimal performance.  
- **Generic Implementation:** Works with any `Comparable` objects.  
- **Efficient Access:** Provides O(1) access to the most recent tweets.  

#### Key Methods in `MyHeap`:  

- **`add`**: Adds new tweets while maintaining heap property.  
- **`delete`**: Removes and returns the most recent tweet.  
- **`peek`**: Views the most recent tweet without removal.  
- **`isEmpty`**: Checks if the heap contains any tweets.  

#### Error Handling Methods:  

- Input validation and error reporting.  
- Exception management for heap operations.  
- Null pointer handling.  

---

## Usage  

1. **Prepare Data File:** Place `tweets_train.tsv` in the correct directory.  
2. **Run Program:** Execute `Program9` to start the system.  
3. **Review Options:**  

   - Sign in with User ID.  
   - View the most recent tweet.  
   - Delete the most recent tweet.  
   - View other users' tweets.  
   - Sign out.  

---

## Example Output  

```plaintext
====================================
    Welcome to TweetMap System
====================================
Version: 1.0
Author: Jered Kalombo
Date: December 2024
====================================


MAIN MENU
1. Start TweetMap Interface
2. About Program
3. Exit Program

Enter your choice (1-3):
