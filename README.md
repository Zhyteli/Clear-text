
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        System.out.println("Введите ваш текст:");
        Scanner wor = new Scanner(System.in);
        String word = wor.nextLine();
        String space = " ";

        for (int i = 0; i < word.length(); i++){
            char ser = word.charAt(i);
            int search = (int) ser;
            if (65 <= search && search <= 90 || search >= 97 && search <= 122 || search == 32){
                space += ser;
            }
        }
        System.out.println("Очищенный текст:" + space);
    }

}
