import java.time.LocalDate;
import java.time.Period;

public class AgeCalculator {
    public static void main(String[] args) {
        // Replace these values with your birthdate
        int birthYear = 1990;
        int birthMonth = 5;
        int birthDay = 11;

        // Get the current date
        LocalDate currentDate = LocalDate.now();

        // Create LocalDate object for birthdate
        LocalDate birthDate = LocalDate.of(birthYear, birthMonth, birthDay);

        // Calculate the period between the birthdate and current date
        Period period = Period.between(birthDate, currentDate);

        // Extract years, months, and days from the period
        int years = period.getYears();
        int months = period.getMonths();
        int days = period.getDays();

        // Print the result
        System.out.println("Your age is: " + years + " years, " + months + " months, and " + days + " days.");
    }
}

