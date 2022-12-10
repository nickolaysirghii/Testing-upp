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
