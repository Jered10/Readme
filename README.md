# Tweet Sorting Analysis Program
This project implements and analyzes different sorting algorithms (QuickSort and RadixSort) for processing tweet data. The system compares performance metrics across different dataset sizes and provides insights into sorting efficiency.

## Purpose
The program's main objective is to analyze and compare the performance of different sorting algorithms when handling tweet datasets. It specifically examines QuickSort and RadixSort implementations, tracking execution times and evaluating their effectiveness with varying data sizes.

# Features

Generic QuickSort Implementation: Custom implementation with median-of-three optimization
Specialized RadixSort: Optimized for sorting tweet IDs
Performance Tracking: Detailed timing measurements for each sort operation
Multiple Dataset Support: Handles both small (80K) and large (1.52M) tweet datasets
Comparative Analysis: Direct comparison of sorting algorithm performance


### Components
#### MyQuickSort Class

Generic Implementation: Works with any Comparable objects
Optimizations:

Median-of-three pivot selection
Hoare's partitioning scheme


Dynamic Comparator: Supports different sorting criteria (ID, datetime)

#### MyRadixSort Class

Specialized for Integers: Optimized for tweet ID sorting
Linear Time Complexity: O(d*n) where d is the number of digits
Space Efficient: Minimizes additional memory usage

#### Tweet Class

Core Data Structure: Represents tweet information
Comparable Interface: Supports natural ordering
Key Attributes: ID, datetime, user, sentiment, text


##### Performance Analysis
Small Dataset (80,000 tweets)
plaintextCopyQuickSort (ID): 56ms (first run)
QuickSort (ID): 97ms (second run)
RadixSort (ID): 31ms
Large Dataset (1,520,000 tweets)
plaintextCopyQuickSort (ID): 527ms (first run)
QuickSort (ID): 692ms (second run)
RadixSort (ID): 608ms

#### Program10 Class

Main Driver Class: Orchestrates the sorting operations
Features:

Loads tweet data from TSV files
Implements comparison of sorting algorithms
Manages timing measurements


#### Usage

Prepare your tweet dataset in TSV format
Compile the program:
bashCopyjavac twitterpack/*.java




### Implementation Details

Program performs multiple sorting operations
Tracks and displays execution times
Shows top 10 sorted tweets
Provides stability analysis
Compares algorithm efficiency


# Author
Jered Kalombo
Version: December 2024
