//Implement a function that finds the maximum element in an array using linar search 

public class MaxElementFinder {

    // Function to find the maximum element using linear search
    public static int findMax(int[] arr) {
        if (arr == null || arr.length == 0) {
            throw new IllegalArgumentException("Array is empty or null");
        }

        int max = arr[0]; // Assume first element is the maximum initially

        // Traverse the array to find the actual maximum
        for (int i = 1; i < arr.length; i++) {
            if (arr[i] > max) {
                max = arr[i];
            }
        }

        return max;
    }

    public static void main(String[] args) {
        int[] array = {5, 2, 8, 1, 9, 3};
        int maxElement = findMax(array);
        System.out.println("Maximum element in the array is: " + maxElement);
    }
}
