# COURIER-TRACKING
import java.util.Scanner;

public class Tracking {

    int id;
    String customer;

    
    Tracking() {
        id = 0;
        customer = "NULL";
    }

    Tracking(int i, String c) {
        id = i;
        customer = c;
    }

    void display() {
        System.out.println("Courier ID : " + id);
        System.out.println("Customer Name : " + customer);
    }

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        Tracking c1 = new Tracking();
        c1.display();

        System.out.print("\nEnter Courier ID: ");
        int id = sc.nextInt();

        System.out.print("Enter Customer Name: ");
        sc.nextLine();
        String name = sc.nextLine();

        Tracking c2 = new Tracking(id, name);
        c2.display();

        sc.close();
    }
}