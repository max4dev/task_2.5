# task_2.5

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        int a = 0;
        String b = "";
        Scanner scan = new Scanner(System.in);
        System.out.print("Введите целое число: ");

        while (scan.hasNext()) {

              while (scan.hasNextInt()) {
                  a = scan.nextInt();
                  if (a == 10) {
                      System.out.print ("Верно!");
                      return;
                  }
                  System.out.print ("Неверно! Попробуйте еще раз: ");
              }

              b = scan.next();
              System.out.print ("Введите целое число: ");
        }
    }
}
