# Question-Two
Assignments
// This program asks the user to enter the marks of five units they did last semester,
// calculates the average and displays it on the screen.

import java.util.Scanner;

public class AverageMarks {

    public static void main(String[] args) {

        // Create a Scanner object to read user input.
        Scanner scanner = new Scanner(System.in);

        // Ask the user to enter the marks of five units.
        System.out.println("Enter the marks of five units: ");

        // Create an array to store the marks.
        int[] marks = new int[5];

        // Read the marks from the user.
        for (int i = 0; i < marks.length; i++) {
            marks[i] = scanner.nextInt();
        }

        // Calculate the average of the marks.
        double average = (double) (marks[0] + marks[1] + marks[2] + marks[3] + marks[4]) / 5;

        // Round the average to two decimal places.
        average = Math.round(average * 100) / 100.0;

        // Display the average.
        System.out.println("The average mark is " + average);
    }
}
