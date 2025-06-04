import java.util.Scanner;

public class ReverseNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        // Take input from user
        System.out.print("Enter a number: ");
        int number = sc.nextInt();
        
        int reverse = 0;

        // Logic to reverse the number
        while (number != 0) {
            int digit = number % 10;     // Get last digit
            reverse = reverse * 10 + digit;  // Add digit to reverse
            number = number / 10;        // Remove last digit
        }

        // Print the reversed number
        System.out.println("Reversed number: " + reverse);

        sc.close();
    }
}
