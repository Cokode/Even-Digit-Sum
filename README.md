# Even-Digit-Sum
This program adds up all even numbers given and returns the sum, it returns error message for negative numbers

public class EvenDigitSum {

    public static void main(String[] args) {
        System.out.println(getEvenDigitSum(768971030));
    }

    public static int getEvenDigitSum(int number) {
        if (number < 0) {
            return -1;
        }

        int sumEven = 0;

        while (number > 0) {
            int evenNum = number % 10;
            number /= 10;
            if (evenNum % 2 == 0) {
                sumEven += evenNum;
            }

        }
        return sumEven;
    }
}
