# Simple-Calculator-Made-in-Java
Calculator go brrr

import java.util.Scanner;

public class Calculator{
    public static void main(String [] args){

        Scanner input = new Scanner(System.in);

        System.out.print("Enter First Number: ");
        int firstNum = input.nextInt();

        System.out.print("Enter Second Number: ");
        int secondNum = input.nextInt();

        System.out.print("Enter Operator Choice: ");
        System.out.println("\n1. Addition ");
        System.out.println("2. Subtraction ");
        System.out.println("3. Multiplcation ");
        System.out.println("4. Division ");
        System.out.println("5. Modulus ");
        int operatorChoice = input.nextInt();

        double addition = firstNum + secondNum;
        double subtraction = firstNum - secondNum;
        double multiplication = firstNum * secondNum;
        double division = (double)firstNum / secondNum;
        double modulus = firstNum % secondNum;

        switch (operatorChoice) {
            case 1:
                System.out.println("Result: " + addition);
                break;
            case 2:
                System.out.println("Result: " + subtraction);
                break;
            case 3:
                System.out.println("Result: " + multiplication);
                break;
            case 4:
                    System.out.println("Result: " + division);
                break;
            case 5:
                System.out.println("Result: " + modulus);
                break;
        
            default:
                System.out.println("Error, give select an Operator from 1-5 only.");
                break;
        }
        input.close();
    }
}
