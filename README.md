import java.util.Random;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Random random = new Random();
        int attemptsLimit = 10;
        int totalAttempts = 0;
        int score = 0;

        System.out.println("WELCOME TO THE NUMBER GAME (^>^)");
        System.out.println("Guess the number within " + attemptsLimit + " attempts");
        System.out.println();
        System.out.println("Start >>>");
        System.out.println();

        boolean playAgain = true;
        while (playAgain) {
            System.out.print("Enter the maximum number: ");
            int maxRange = sc.nextInt();
            System.out.print("Enter the minimum number: ");
            int minRange = sc.nextInt();
            System.out.println("Guess a number between " + minRange + " and " + maxRange + ".");

            int targetNumber = random.nextInt(maxRange - minRange + 1) + minRange;
            int attempts = 0;
            boolean guessedCorrectly = false;

            while (attempts < attemptsLimit && !guessedCorrectly) {
                System.out.print("Enter your guess: ");
                int userGuess = sc.nextInt();
                attempts++;
                totalAttempts++;

                if (userGuess == targetNumber) {
                    System.out.println("Congratulations! You guessed the correct number in " + attempts + " attempts.");
                    score++;
                    guessedCorrectly = true;
                } else if (userGuess < targetNumber) {
                    System.out.println("Too low. Try again.");
                } else {
                    System.out.println("Too high. Try again.");
                }
            }

            if (!guessedCorrectly) {
                System.out.println("Sorry, you have reached the maximum attempts.");
                System.out.println("The correct number was: " + targetNumber);
            }

            System.out.println("Your current score: " + score);
            double scorerate = (double) score / totalAttempts * 100;
            System.out.printf("Your scorerate is %.2f%%\n", scorerate);
            System.out.println();
            System.out.print("Do you want to play again? (yes/no): ");
            String playChoice = sc.next().toLowerCase();
            if (!playChoice.equals("yes")) {
                System.out.print("Enter new game? (yes/no): ");
                String newGameChoice = sc.next().toLowerCase();
                if (!newGameChoice.equals("yes")) {
                    playAgain = false;
                }
            }
        }

        System.out.println("Thanks for playing^~^");
        System.out.println();
        
        System.out.println("Your final score: " + score);
        double finalScorerate = (double) score / totalAttempts * 100;
        System.out.printf("Your final score rate: %.2f%%\n", finalScorerate);

        sc.close();
    }
}
import java.util.Random;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Random random = new Random();
        int attemptsLimit = 10;
        int totalAttempts = 0;
        int score = 0;

        System.out.println("WELCOME TO THE NUMBER GAME (^>^)");
        System.out.println("Guess the number within " + attemptsLimit + " attempts");
        System.out.println();
        System.out.println("Start >>>");
        System.out.println();

        boolean playAgain = true;
        while (playAgain) {
            System.out.print("Enter the maximum number: ");
            int maxRange = sc.nextInt();
            System.out.print("Enter the minimum number: ");
            int minRange = sc.nextInt();
            System.out.println("Guess a number between " + minRange + " and " + maxRange + ".");

            int targetNumber = random.nextInt(maxRange - minRange + 1) + minRange;
            int attempts = 0;
            boolean guessedCorrectly = false;

            while (attempts < attemptsLimit && !guessedCorrectly) {
                System.out.print("Enter your guess: ");
                int userGuess = sc.nextInt();
                attempts++;
                totalAttempts++;

                if (userGuess == targetNumber) {
                    System.out.println("Congratulations! You guessed the correct number in " + attempts + " attempts.");
                    score++;
                    guessedCorrectly = true;
                } else if (userGuess < targetNumber) {
                    System.out.println("Too low. Try again.");
                } else {
                    System.out.println("Too high. Try again.");
                }
            }

            if (!guessedCorrectly) {
                System.out.println("Sorry, you have reached the maximum attempts.");
                System.out.println("The correct number was: " + targetNumber);
            }

            System.out.println("Your current score: " + score);
            double scorerate = (double) score / totalAttempts * 100;
            System.out.printf("Your scorerate is %.2f%%\n", scorerate);
            System.out.println();
            System.out.print("Do you want to play again? (yes/no): ");
            String playChoice = sc.next().toLowerCase();
            if (!playChoice.equals("yes")) {
                System.out.print("Enter new game? (yes/no): ");
                String newGameChoice = sc.next().toLowerCase();
                if (!newGameChoice.equals("yes")) {
                    playAgain = false;
                }
            }
        }

        System.out.println("Thanks for playing^~^");
        System.out.println();
        
        System.out.println("Your final score: " + score);
        double finalScorerate = (double) score / totalAttempts * 100;
        System.out.printf("Your final score rate: %.2f%%\n", finalScorerate);

        sc.close();
    }
}
import java.util.Random;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Random random = new Random();
        int attemptsLimit = 10;
        int totalAttempts = 0;
        int score = 0;

        System.out.println("WELCOME TO THE NUMBER GAME (^>^)");
        System.out.println("Guess the number within " + attemptsLimit + " attempts");
        System.out.println();
        System.out.println("Start >>>");
        System.out.println();

        boolean playAgain = true;
        while (playAgain) {
            System.out.print("Enter the maximum number: ");
            int maxRange = sc.nextInt();
            System.out.print("Enter the minimum number: ");
            int minRange = sc.nextInt();
            System.out.println("Guess a number between " + minRange + " and " + maxRange + ".");

            int targetNumber = random.nextInt(maxRange - minRange + 1) + minRange;
            int attempts = 0;
            boolean guessedCorrectly = false;

            while (attempts < attemptsLimit && !guessedCorrectly) {
                System.out.print("Enter your guess: ");
                int userGuess = sc.nextInt();
                attempts++;
                totalAttempts++;

                if (userGuess == targetNumber) {
                    System.out.println("Congratulations! You guessed the correct number in " + attempts + " attempts.");
                    score++;
                    guessedCorrectly = true;
                } else if (userGuess < targetNumber) {
                    System.out.println("Too low. Try again.");
                } else {
                    System.out.println("Too high. Try again.");
                }
            }

            if (!guessedCorrectly) {
                System.out.println("Sorry, you have reached the maximum attempts.");
                System.out.println("The correct number was: " + targetNumber);
            }

            System.out.println("Your current score: " + score);
            double scorerate = (double) score / totalAttempts * 100;
            System.out.printf("Your scorerate is %.2f%%\n", scorerate);
            System.out.println();
            System.out.print("Do you want to play again? (yes/no): ");
            String playChoice = sc.next().toLowerCase();
            if (!playChoice.equals("yes")) {
                System.out.print("Enter new game? (yes/no): ");
                String newGameChoice = sc.next().toLowerCase();
                if (!newGameChoice.equals("yes")) {
                    playAgain = false;
                }
            }
        }

        System.out.println("Thanks for playing^~^");
        System.out.println();
        
        System.out.println("Your final score: " + score);
        double finalScorerate = (double) score / totalAttempts * 100;
        System.out.printf("Your final score rate: %.2f%%\n", finalScorerate);

        sc.close();
    }
}
import java.util.Random;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Random random = new Random();
        int attemptsLimit = 10;
        int totalAttempts = 0;
        int score = 0;

        System.out.println("WELCOME TO THE NUMBER GAME (^>^)");
        System.out.println("Guess the number within " + attemptsLimit + " attempts");
        System.out.println();
        System.out.println("Start >>>");
        System.out.println();

        boolean playAgain = true;
        while (playAgain) {
            System.out.print("Enter the maximum number: ");
            int maxRange = sc.nextInt();
            System.out.print("Enter the minimum number: ");
            int minRange = sc.nextInt();
            System.out.println("Guess a number between " + minRange + " and " + maxRange + ".");

            int targetNumber = random.nextInt(maxRange - minRange + 1) + minRange;
            int attempts = 0;
            boolean guessedCorrectly = false;

            while (attempts < attemptsLimit && !guessedCorrectly) {
                System.out.print("Enter your guess: ");
                int userGuess = sc.nextInt();
                attempts++;
                totalAttempts++;

                if (userGuess == targetNumber) {
                    System.out.println("Congratulations! You guessed the correct number in " + attempts + " attempts.");
                    score++;
                    guessedCorrectly = true;
                } else if (userGuess < targetNumber) {
                    System.out.println("Too low. Try again.");
                } else {
                    System.out.println("Too high. Try again.");
                }
            }

            if (!guessedCorrectly) {
                System.out.println("Sorry, you have reached the maximum attempts.");
                System.out.println("The correct number was: " + targetNumber);
            }

            System.out.println("Your current score: " + score);
            double scorerate = (double) score / totalAttempts * 100;
            System.out.printf("Your scorerate is %.2f%%\n", scorerate);
            System.out.println();
            System.out.print("Do you want to play again? (yes/no): ");
            String playChoice = sc.next().toLowerCase();
            if (!playChoice.equals("yes")) {
                System.out.print("Enter new game? (yes/no): ");
                String newGameChoice = sc.next().toLowerCase();
                if (!newGameChoice.equals("yes")) {
                    playAgain = false;
                }
            }
        }

        System.out.println("Thanks for playing^~^");
        System.out.println();
        
        System.out.println("Your final score: " + score);
        double finalScorerate = (double) score / totalAttempts * 100;
        System.out.printf("Your final score rate: %.2f%%\n", finalScorerate);

        sc.close();
    }
}
import java.util.Random;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Random random = new Random();
        int attemptsLimit = 10;
        int totalAttempts = 0;
        int score = 0;

        System.out.println("WELCOME TO THE NUMBER GAME (^>^)");
        System.out.println("Guess the number within " + attemptsLimit + " attempts");
        System.out.println();
        System.out.println("Start >>>");
        System.out.println();

        boolean playAgain = true;
        while (playAgain) {
            System.out.print("Enter the maximum number: ");
            int maxRange = sc.nextInt();
            System.out.print("Enter the minimum number: ");
            int minRange = sc.nextInt();
            System.out.println("Guess a number between " + minRange + " and " + maxRange + ".");

            int targetNumber = random.nextInt(maxRange - minRange + 1) + minRange;
            int attempts = 0;
            boolean guessedCorrectly = false;

            while (attempts < attemptsLimit && !guessedCorrectly) {
                System.out.print("Enter your guess: ");
                int userGuess = sc.nextInt();
                attempts++;
                totalAttempts++;

                if (userGuess == targetNumber) {
                    System.out.println("Congratulations! You guessed the correct number in " + attempts + " attempts.");
                    score++;
                    guessedCorrectly = true;
                } else if (userGuess < targetNumber) {
                    System.out.println("Too low. Try again.");
                } else {
                    System.out.println("Too high. Try again.");
                }
            }

            if (!guessedCorrectly) {
                System.out.println("Sorry, you have reached the maximum attempts.");
                System.out.println("The correct number was: " + targetNumber);
            }

            System.out.println("Your current score: " + score);
            double scorerate = (double) score / totalAttempts * 100;
            System.out.printf("Your scorerate is %.2f%%\n", scorerate);
            System.out.println();
            System.out.print("Do you want to play again? (yes/no): ");
            String playChoice = sc.next().toLowerCase();
            if (!playChoice.equals("yes")) {
                System.out.print("Enter new game? (yes/no): ");
                String newGameChoice = sc.next().toLowerCase();
                if (!newGameChoice.equals("yes")) {
                    playAgain = false;
                }
            }
        }

        System.out.println("Thanks for playing^~^");
        System.out.println();
        
        System.out.println("Your final score: " + score);
        double finalScorerate = (double) score / totalAttempts * 100;
        System.out.printf("Your final score rate: %.2f%%\n", finalScorerate);

        sc.close();
    }
}
# CodSoft
My Internship tasks
