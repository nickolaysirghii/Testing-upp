package org.Nicolay;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

            Scanner scanner = new Scanner(System.in);
            int digit = scanner.nextInt();
            System.out.println(secondStep(digit));
            System.out.println(thirdStep(digit));
            System.out.println(forthStep(digit));

        }
        public static int secondStep(int digit){
            int first = digit / 100;
            return first;
        }
        public static int thirdStep(int digit){
            int second = digit % 100 / 10;
            return second;
        }
        public static int forthStep(int digit){
            int third = digit % 110 % 10;
            return third;
        }

    }
