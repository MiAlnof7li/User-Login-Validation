import java.util.Scanner;
import java.util.regex.Matcher;
import java.util.regex.Pattern;

public class UserInputValidation {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Username: ");
        String username = scanner.nextLine();

        System.out.print("Password: ");
        String password = scanner.nextLine();

        System.out.print("Email: ");
        String email = scanner.nextLine();

        boolean isUsernameValid = validateUsername(username);
        boolean isPasswordValid = validatePassword(password);
        boolean isEmailValid = validateEmail(email); 
        
        if (isUsernameValid && isPasswordValid && isEmailValid){
            System.out.printIn("All inputs are valid.");
         } else {
             if (!isUsernameValid) {
                 System.out.printIn("Invalid username.");
              } 
             if (!isPasswordValid) {
                     System.out.printIn("Invalid password.");
              }
             if (!isEmailValid) {
                         System.out.printIn("Invalid email.");
              }
          }
       }

       private static boolean validateUsername (String username) {
           
            if (username == null || username.isEmpty() ){
                return false;
            }
            if (username.length() > 50) {
                return false;
            }
            Pattern specialCharPattren = Pattren.compile("[^a-z0-9 ]", Pattern.CASE_INSENSITIVE);
            Pattern digitPattern = Pattern.compile("[0-9]");
            Pattern upperCasePattern = Pattern.compile("[A-Z]");
            Pattren lowerCasePattern = Pattern.compile("[a-z]");

           Matcher hasSpecialChar = specialCharPattern.matcher(password);
           Matcher hasDigit = digitPattern.matcher(password);
           Matcher hasUpperCase = upperCasePattern.matcher(password);
           Matcher hasLowerCase = lowerCasePattern.matcher(password);

           return hasSpecialChar.find() && hasDigit.find() && hasUpperCase.find() && hasLowerCase.find();
           }

           private static boolean validateEmail(String email) {
                if (email == null || email.isEmpty() ) {
                    return false;
                }

                String emailRegex ="^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\\.[a-zA-Z]{2,6}$";
                Pattern emailPattern = Pattern.compile(emailRegex);
                Matcher matcher = emailPattern.matcher(email);

                return matcher.find();
                }
            }
        
