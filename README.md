# HCF
highest common factor in java
import java.util.Scanner;

public class HCF {
    public HCF() {
    }

    static int HCF(int a, int b) {
        return b == 0 ? a : HCF(b, a % b);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter a: ");
        int a = sc.nextInt();
        System.out.println("Enter b; ");
        int b = sc.nextInt();
        System.out.println("HCF(" + a + "," + b + ")= " + HCF(a, b));
    }
}
