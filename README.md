package org.Nicolay;

import org.junit.Assert;
import org.junit.Test;

import static org.junit.Assert.*;

public class MainTest {
    @Test
    public void test() {
        int answer = Main.secondStep(234);
        assertEquals(2, answer);
    }

    @Test
    public void test2() {
        int answer = Main.thirdStep(234);
        assertEquals(3, answer);
    }

    @Test
    public void test3() {
        int answer = Main.forthStep(234);
        assertEquals(4, answer);

    }
}
....................................................................................................................................................
,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
....................................................................................................................................................
the basic code .
/////

import java.util.Scanner;

// public class Main {
//    public static void main(String[] args) {
//        Scanner x = new Scanner(System.in);
//        int digit = x.nextInt();
//        int first = digit / 100;
//        int second = digit % 100 / 10;
//        int third = digit % 110 % 10;
//        System.out.println(first);
//        System.out.println(second);
//        System.out.println(third);
//
//
//    }
//}
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
