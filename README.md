# Calcus
//GrandFatherCalculator
import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("your number is a-");

        double a = sc.nextDouble();
        System.out.println("your number is b-");
        double b = sc.nextDouble();
        System.out.println("Select Operation: + 1, - 2, * 3, / 4");
        int operation = sc.nextInt();

        double result =0;
        if(operation ==1){
            result = totality(a,b);
        } else if (operation ==2) {
            result = minusirovka(a,b);
        } else if (operation ==3) {
            result = hasilality(a,b);
        } else if (operation == 4) {
            result = bolarity(a,b);
        } else {
            System.out.println("operation is not valid");
        }
        System.out.println("result="+result);


    }
    public static double totality( double a, double b){
        return a+b;

    }

    public static double minusirovka (double a, double b) {
        return a-b;
    }

    public static double hasilality (double a, double b){
        return a*b;
    }
    public static double bolarity (double a,double b){
        return a/b;
    }

}
