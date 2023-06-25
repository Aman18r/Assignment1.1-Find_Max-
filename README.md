# Assignment1.1-Find_Max-

import java.util.Scanner;
public class Main{

    static int findMax(int[] arr){
        int max = Integer.MIN_VALUE;
        for(int i = 0; i < arr.length; i++){
            if(arr[i] > max){
                max = arr[i];
            }
        }
        return max;
    }
    public static void main(String[] args) {
            Scanner sc = new Scanner(System.in);
        System.out.println("Enter the size of an array: ");
            int a = sc.nextInt();
            int[] arr = new int[a];

        System.out.println("Enter " + a + " elements");
            for(int i = 0; i < a; i++){
                arr[i] = sc.nextInt();
            }
        System.out.println("Maximum Element is: " + findMax(arr));
    }
}
