# Tap Tap Game

import java.util.Scanner;

public class TapTapGame {
    private static int score = 0;
    private static int targetScore = 10;

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Welcome to the Tap Tap Game!");
        System.out.println("Press 'Enter' to tap!");

        while (score < targetScore) {
            scanner.nextLine();
            score++;
            System.out.println("Score: " + score);
        }

        System.out.println("Congratulations! You've reached the target score of " + targetScore + "!");
        scanner.close();
    }
}
