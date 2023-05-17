
Sorts an array using the Insertion Sort algorithm.
for the parameters {Array} arr - The input array to be sorted.
for the returns {Array} - The sorted array. */
// Traverse through the array starting from the second element for (let i = 1; i < arr.length; i++) { const key = arr[i]; // Element to be inserted into the sorted sequence let j = i - 1; // Index of the last element in the sorted sequence

// Shift elements of the sorted sequence that are greater than the key to the right
while (j >= 0 && arr[j] > key) {
  arr[j + 1] = arr[j];
  j--;
}

arr[j + 1] = key;  // Insert the key into its correct position in the sorted sequence
}

return arr; } In this implementation, I defined a function called insertionSort that takes an input array arr. The each comments in the code explain each step of the algorithm.

As instructed I used two counters, i and j. i represents the current element to be inserted into the sorted sequence, and j is used to compare the key with the elements in the sorted sequence and shift them if necessary.

To use the Insertion Sort algorithm, you can call the insertionSort function with your desired array as an argument. It will return the sorted array.
