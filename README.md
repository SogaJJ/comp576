# comp576

## description of the preprocessed dataset:
### processed_labels_no_criteria_binary.csv: 
calculate the rounded mean value of five scores. set the label to be 0 if the mean value is less than 0, and set to 1 if the value is greater than 1. disregard if the mean value is equal to 0.

### processed_labels_no_criteria.csv: 
label is the rounded mean value. original is from [-3, -2, -1, 0, 1, 2, 3]. transform to [0, 1, 2, 3, 4, 5, 6] by adding 3 to each value. This is easy for training.

### processed_labels_no_criteria_three_class.csv: 
calculate the mean value of five scores. set the label to be 2 if the mean value is larger than 1, and set to 0 if the value is less than -1. Otherwise, set to 1.

### processed_labels_no_criteria_binary_filtered.csv: 
remove sample with variance larger than 1, calculate the rounded mean value of five scores. set the label to be 0 if the mean value is less than 0, and set to 1 if the value is greater than 1. disregard if the mean value is equal to 0.
