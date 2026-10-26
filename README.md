import java.util.Scanner;

public class WordCount {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Enter the text:");
        String text = sc.nextLine();

        text = text.trim();
        int count = text.isEmpty() ? 0 : text.split("\\s+").length;

        System.out.println("Number of words in the text:" + count);

        sc.close();
    }
}
