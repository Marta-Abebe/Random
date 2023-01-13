# Random
import java.util.Arrays;
import java.util.Random;
import java.util.Scanner;

public class Loops {

    public static void main(String args[]){

      Scanner scanner = new Scanner(System.in);
        System.out.println("please insert a number ");
        int number = scanner.nextInt();

        while (number >= 0){

            if(number%2==0)
                System.out.println(number);
            number--;
        }


        do {
            if(number%2!=0)
                System.out.println(number);
        }while (number< 0);
        System.out.println("please insert the number of members ");
        int memberSize= scanner.nextInt();
        String[] membersList  = new String[memberSize];

        int index =  0;
        while (membersList.length > index ){
            System.out.println("please insert your name ");
            membersList[index] = scanner.next();
            index++;
        }

        System.out.println(Arrays.toString(membersList));
        Random random = new Random();
        int luckyNumber  = random.nextInt(0, memberSize);
        System.out.println(membersList[luckyNumber]);
//



    }


}
