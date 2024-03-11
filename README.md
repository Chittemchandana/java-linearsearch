# java-linearsearch
# ALGORITHM for Linear Search
# Step 1: Start 
# Step 2: Declare an array and search element as key.
# Step 3: Traverse the array until the number is found.
# Step 4: If the key element is found, return the index position of the array element
# Step 5: If the key element is not found, return -1
# Step 6: Stop.

# approach1
public int linearSearch(int[] arr, int x) {
    for (int i = 0; i < arr.length; i++) {
        if (arr[i] == x) {
            return i;
        }
    }
    return -1; // element not found
}

# approach2
// Java code for linearly search x in arr[]. If x 
// is present then return its location, otherwise 
// return -1 
class LinearSearch { 
	// This function returns index of element x in arr[] 
	static int search(int arr[], int n, int x) 
	{ 
		for (int i = 0; i < n; i++) { 
			// Return the index of the element if the element 
			// is found 
			if (arr[i] == x) 
				return i; 
		} 

		// return -1 if the element is not found 
		return -1; 
	} 

	public static void main(String[] args) 
	{ 
		int[] arr = { 3, 4, 1, 7, 5 }; 
		int n = arr.length; 
		
		int x = 4; 

		int index = search(arr, n, x); 
		if (index == -1) 
			System.out.println("Element is not present in the array"); 
		else
			System.out.println("Element found at position " + index); 
	} 
} 
