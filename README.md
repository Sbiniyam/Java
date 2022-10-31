# Java
Java code on microfinance
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
       Scanner scan = new Scanner(System.in);
        System.out.print("Welcome to our company. Please insert your name: ");
        String name = scan.nextLine().trim();

        System.out.print("How long do you save in our company(Please fill in month)? ");
        int membershipTime = scan.nextInt();
        if (membershipTime >= 6){
            System.out.println("You are eligibile to borrow.");
            System.out.print("How much do you have on your saving account? ");
            int amountOnSavingAccount = scan.nextInt();
            System.out.print("How much money do you want to borrow? ");
            int moneyToBeBorrowed = scan.nextInt();
            String eligibilityOfAskedMoney = amountOnSavingAccount >= (moneyToBeBorrowed * 0.25) ? "You are eligibible to borrow the money you asked." : "Sorry, due to your saving you can not borrow the money you requested.";
                System.out.println(eligibilityOfAskedMoney);
            System.out.println("Insert your criminal record");
            String criminal = scan.nextLine();
            if (criminal == "YES")
                    System.out.println("you are not allowed");

            }
        else
            {
                System.out.println("Sorry, your saving period is less than six month. So you are not eligible to borrow.");
            }
