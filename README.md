# Twitter Sentiment Analysis Program  

This project provides a robust system for analyzing sentiment in Twitter data using a custom **HashMap** implementation. By leveraging an efficient data structure and sentiment analysis model, the program processes large datasets of tweets, measures performance metrics, and evaluates sentiment prediction accuracy.  

The system includes comprehensive performance tracking, reporting build times, and hash map efficiency through resize operations.  

---

## Purpose  

The purpose of this program is to enable efficient sentiment analysis of tweets using a custom **HashMap-based implementation**. The program processes training and test datasets, builds a sentiment analysis model, and evaluates prediction accuracy while tracking performance metrics.  

Users can analyze the system's efficiency through measurements of data loading times and hash map resize operations.  

---

## Features  

- **Custom HashMap Implementation:** Efficient storage and retrieval of tweet data with dynamic resizing capabilities.  
- **Performance Tracking:** Detailed monitoring of build times and resize operations.  
- **Sentiment Analysis Model:** Trains on labeled data to make accurate predictions.  
- **Error Handling:** Comprehensive handling of file I/O operations.  
- **Metrics Reporting:** Real-time performance measurement and reporting.  

---

## Components  

### **Tweet Class**  
The `Tweet` class represents a tweet with its content and associated metadata, designed to work seamlessly with the custom HashMap implementation for efficient storage and retrieval.  

### **MyHashMap Class**  

- **Dynamic Resizing:** Automatically adjusts size for optimal performance.  
- **Performance Monitoring:** Tracks resize operations and build times.  
- **Generic Implementation:** Handles `Tweet` objects mapped to Boolean sentiment values.  
- **Efficient Storage:** Optimized data structure for quick access and updates.  

#### Key Methods in `MyHashMap`:  

- **`readDataToHashMap`**: Processes and loads tweet data from TSV files.  
- **`getResizeCount`**: Returns the number of resize operations performed.  
- **`prediction`**: Calculates and returns sentiment prediction accuracy.  

#### Error Handling Methods:  

- Comprehensive file operation error handling.  
- Data validation and error reporting.  
- Exception management for I/O operations.  

---

## Usage  

1. **Prepare Data Files:** Place `tweets_train.tsv` and `tweets_test.tsv` in the correct directory.  
2. **Run Program:** Execute `Program8` to begin data processing.  
3. **Review Output:** Analyze the following metrics:  

   - **Training Data Build Time:** Displays milliseconds taken to build the training hash map.  
   - **Test Data Build Time:** Displays milliseconds taken to build the test hash map.  
   - **Hash Map Resize Counts:** Shows the number of resizing operations for each hash map.  
   - **Prediction Accuracy Ratio:** Outputs the ratio of correct predictions made by the model.  

---

## Example Output  

```plaintext
Build Times:  
- Training Hash Map: 125ms  
- Testing Hash Map: 98ms  

Resize Counts:  
- Training Hash Map: 4  
- Testing Hash Map: 3  

Prediction Results:  
- Accuracy: 87.5%


Author

Jered Kalombo
Version: 26 November 2024
