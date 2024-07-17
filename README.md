[ReverseString.txt](https://github.com/user-attachments/files/16262758/ReverseString.txt)[Factorofnumbers.txt](https://github.com/user-attachments/files/16262755/Factorofnumbers.txt)[Calculator.txt](https://github.com/user-attachments/files/16262683/Calculator.txt)# Java-Assessments

Day-1(Q1):
![Screenshot 2024-07-16 215308](https://github.com/user-attachments/assets/84144fd8-30ed-45e6-a269-493fea44f5f0)
[public class Calculator{
    public static double calculate(double a,double b,String operator){
        switch(operator){
            case "+":
                return a + b;
            case "-":
                return a - b;
            case "*":
                return a * b;
            case "/":
                if (b != 0) {
                    return a / b;
                } else {
                    throw new IllegalArgumentException("Division by zero is not allowed.");
                }
            default:
                throw new IllegalArgumentException("Invalid operator");
        }
    }

    public static void main(String[] args) {
        System.out.println("10 + 8 = " + calculate(10, 8, "+"));
        System.out.println("10 - 8 = " + calculate(10, 8, "-"));
        System.out.println("10 * 8 = " + calculate(10, 8, "*"));
        System.out.println("10 / 8 = " + calculate(10, 8, "/"));
    }
}
Uploading Calculator.txt…]()


Day-1(Q2):
![Scre[PrimeNumber.txt](https://github.com/user-attachments/files/16262741/PrimeNumber.txt)
enshotpublic class PrimeNumber{
    public static boolean isPrime(int num){
        if (num <= 1) {
            return false;
        }
        for (int i = 2; i <= Math.sqrt(num); i++) {
            if (num % i == 0) {
                return false;
            }
        }
        return true;
    }

    public static void main(String[] args) {
        System.out.println("Is 18 a prime number? " + isPrime(18));
        System.out.println("Is 184517 a prime number? " + isPrime(184517));
    }
}
 2024-07-16 215549](https://github.com/user-attachments/assets/fc5c1c4b-cde1-425e-aaa1-a09b77ffee8e)


Day-2(Q1):
![Screenshot 2024-07-16 220034](https://github.com/user-attachments/assets/c9e5b1fe-6e0f-4b26-bb66-235856edc2ad)


[Uploading public class Factor{
    public static void printFactors(int num){
        System.out.print("Factors of " + num + " are: ");
        for (int i = 1; i <= num; i++) {
            if (num % i == 0) {
                System.out.print(i + " ");
            }
        }
        System.out.println();
    }

    public static void main(String[] args) {
        printFactors(18); 
        printFactors(45); 
    }
}Factorofnumbers.txt…]()


Day-2(Q2):
![Screenshot 2024-07-16 220529](https://github.com/user-attachments/assets/3047f39d-17a5-46eb-b3c2-d18579f2e893)


[Uploading ReverseString.public class ReverseString{
    public static String reverse(String str){
        String reversed = "";
        for (int i = str.length() - 1; i >= 0; i--) {
            reversed += str.charAt(i);
        }
        return reversed;
    }

    public static void main(String[] args) {
        System.out.println("Reverse of 'virat' is: " + reverse("virat"));
        System.out.println("Reverse of 'ilhok gnik' is: " + reverse("ilhok gnik"));
    }
}txt…]()







