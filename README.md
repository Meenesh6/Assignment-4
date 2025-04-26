import java.util.HashMap;
import java.util.Scanner;

public class HashMapStringKeyExample {
    public static void main(String[] args) {
        // Create a HashMap with String keys
        HashMap<String, String> map = new HashMap<>();

        // Add some key-value pairs
        map.put("A101", "Apple");
        map.put("B202", "Banana");
        map.put("C303", "Cherry");
        map.put("D404", "Date");

        // Display the HashMap
        System.out.println("HashMap: " + map);

        // Get user input for key to search
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter key to search (e.g., A101): ");
        String key = scanner.nextLine();

        // Search for the key
        if (map.containsKey(key)) {
            System.out.println("Key found! Value = " + map.get(key));
        } else {
            System.out.println("Key not found in the HashMap.");
        }

        scanner.close();
    }
}# Assignment-4
