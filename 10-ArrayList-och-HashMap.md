Läs dessa sidor på W3Schools:

* https://www.w3schools.com/java/java_arraylist.asp
* https://www.w3schools.com/java/java_hashmap.asp
* https://www.w3schools.com/java/java_wrapper_classes.asp

## Exempel från video 2021-10-14

```java
import java.util.ArrayList;

public class ArrayListExample {
    public static void main(String[] args) {
        ArrayList<Integer> myFavoriteNumbers = new ArrayList<Integer>();

        myFavoriteNumbers.add(1); // Add the number 1 to the ArrayList.
                                  // This is our first element so it will get index 0.
        myFavoriteNumbers.set(0, 5); // Change index 0 to number 5

        // A regular for-loop as we've used it before
        for(int i = 0; i < myFavoriteNumbers.size(); i++) {
            // Note: We're using .get(index) instead of []
            System.out.println(myFavoriteNumbers.get(i));
        }

        // Same as the for-loop above - but you don't get the index number which sometimes
        // is very useful
        // This is a "for each" loop. If you say this out loud you say "For each number in myFavoriteNumbers"
        for (Integer number : myFavoriteNumbers) {
            System.out.println(number);
        }

        // Same thing as above but with regular old arrays
        int[] myArray = new int[10];
        int myArrayIndex0 = myArray[0];
        myArray[0] = 5;
    }
}
```