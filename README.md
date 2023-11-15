# turing-machine-in-jflap
import java.util.Random;

public class RandomABString {
    public static void main(String[] args) {
        int length = 10; // Change this to the desired length of the string
        Random random = new Random();

        StringBuilder result = new StringBuilder();

        // Add random 'a's to the string
        for (int i = 0; i < length; i++) {
            if (random.nextBoolean()) {
                result.append('a');
            }
        }

        // Add random 'b's to the string
        for (int i = 0; i < length; i++) {
            if (random.nextBoolean()) {
                result.append('b');
            }
        }

        System.out.println(result.toString());
    }
}
