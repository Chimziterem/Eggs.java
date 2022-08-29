# Eggs.java

import java.util.Scanner;
class Eggs {
    public static void main(String[] args) {
       final int dozen = 12;
        double price_dozen = 3.25;
        double loose_egg_price = 0.45;
        String number_of_eggs;
        Scanner input = new Scanner(System.in);
int eggs;
        
        System.out.print("Enter number of eggs needed >> ");
        eggs = input.nextInt();
        int number_of_dozen = eggs/dozen;
        int number_of_loose_egg = eggs%dozen;
        double total_price =  (number_of_dozen * price_dozen) + (number_of_loose_egg * loose_egg_price);

        System.out.println("You ordered "+eggs+" eggs. That's "+number_of_dozen+" dozen at $3.25 per dozen and "+number_of_loose_egg+" loose eggs at " +
                "45 cents each for a total of $"+total_price+".");
    
    
    }
    }
