import java.util.Scanner; //Aaron Castillo

public class ShoppingList {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String[] shoppingList = new String[5];
        int count = 0;

        System.out.println("Enter up to 5 items to buy:");
        for (int i = 0; i < 5; i++) {
            System.out.print("> Item " + (i + 1) + ": ");
            String item = sc.nextLine().trim();
            if (!item.isEmpty()) {
                shoppingList[count] = item;
                count++;
            }
        }

        // Print the shopping list
        System.out.println("\nYour shopping list:");
        for (int i = 0; i < count; i++) {
            System.out.print(shoppingList[i]);
            if (i < count - 1) System.out.print(", ");
        }

        // Print number of items
        System.out.println("\n\nYou entered " + count + " items.");

        // Search feature
        System.out.print("\nSearch for an item: ");
        String searchItem = sc.nextLine();
        boolean found = false;

        for (int i = 0; i < count; i++) {
            if (shoppingList[i].equalsIgnoreCase(searchItem)) {
                found = true;
                break;
            }
        }

        if (found) {
            System.out.println("✅ " + searchItem + " is in your shopping list!");
        } else {
            System.out.println("❌ " + searchItem + " is NOT in your shopping list.");
        }

        sc.close();
    }
    
