
import java.util.Scanner;

public class ElectricityBill {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter units consumed: ");
        double units = scanner.nextDouble();
        scanner.close();

        double bill;

        if (units <= 50) {
            bill = units * 0.50;
        } else if (units <= 100) {
            bill = 25 + ((units - 50) * 0.75);
        } else if (units <= 200) {
            bill = 25 + 25 + ((units - 100) * 1.20);
        } else {
            bill = 25 + 25 + 60 + ((units - 200) * 1.50);
        }

        System.out.println("Electricity Bill: " + bill);
    }
}
Output:


Enter units consumed: 120
Electricity Bill: 81.0
# Electricity-bill-program-
