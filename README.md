# program-1.java
import java.util.Scanner;

public class JavaExample {

    public static void main(String[] args) {

    	double a, b;
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter first number:");
        a = sc.nextDouble();
        System.out.print("Enter second number:");
        b = sc.nextDouble();

        System.out.print("Enter an operator (+, -, *, /): ");
        char operator = sc.next().charAt(0);

        scanner.close();
        double output;

        switch(operator)
        {
            case '+':
            	output = a + b;
                break;

            case '-':
            	output = a - b;
                break;

            case '*':
            	output =  a * b;
                break;

            case '/':
            	output =  a / b;
                break;

            /* If user enters any other operator or char apart from
             * +, -, * and /, then display an error message to user
             * 
             */
            default:
                System.out.println("You have entered wrong operator");
                return;
        }

        System.out.println(a+" "+operator+" "+b+": "+output);
    }
}
