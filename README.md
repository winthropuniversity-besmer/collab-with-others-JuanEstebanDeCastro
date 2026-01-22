# collab-with-others-JuanEstebanDeCastro
Hello My name is juan I am cool
Hello Everybody, My name is Markiplier
Juan(the sigma) found an ancient city in MC
/*   
    Ryan Orjuela
    October 1st, 2025
    Programming Assignment 1: Sorting Analysis
*/
  
import java.util.*;

public class SortAnal {
    // Sorting the Analysis counter correction from Levitin 2.6 example
    public static int SortAnalCounter(int[] arr) {
        int count = 0;
        int n = arr.length;
        for(int i = 1; i <= n - 1; i++){
            int v = arr[i];
            int j = i - 1;
            while(j >= 0){
                count = count + 1;
                if(arr[j] > v) {
                arr[j + 1] = arr[j];
                j = j - 1; 
                }
                    else {
                        break;
                    }
                }
            arr[j + 1] = v;
        }
            return count;
    }

    public static void main (String[] args) {

        try{
    // generate arrays
            System.out.println("Size, Random Counter\t");
            Random random = new Random();
                // Random Array 
                for(int size = 1000; size <= 20000; size += 1000){
                    int[] randomArr = new int[size]; // Input the creation of the Random Array to Size
                    for(int i = 0; i < size; i++) {
                        // Input of the next variable of the size from 1000-20000
                        randomArr[i] = random.nextInt();
                    }
                    // random array counter into the size from 1000-20000
                    int randomCounter = SortAnalCounter(randomArr);
                    // print
                    System.out.println(size + ", " + randomCounter);
                } 
            System.out.println("Size, Ascending Counter\t");
            // Ascending Array
               for(int size = 1000; size <= 20000; size += 1000){
                    int[] ascArr = new int[size]; // Input the creation of the Ascending Array to Size
                    for(int i = 0; i < size; i++) {
                        // Input of Ascending Array dicussed in class of A[i] = i
                        ascArr[i] = i;
                    }

                    // random array counter into the size from 1000-20000
                    int ascCounter = SortAnalCounter(ascArr);
                    // print
                    System.out.println(size + ", " + ascCounter);
                } 

            System.out.println("Size, Descending Counter\t");
            // Descending Array
                for(int size = 1000; size <= 20000; size += 1000){
                    int[] descArr = new int[size]; // Input the creation of the Ascending Array to Size
                    for(int i = 0; i < size; i++) {
                        // Input of Descending Array dicussed in class of A[i] = -i
                        descArr[i] = -i;
                    }
                    // random array counter into the size from 1000-20000
                    int descCounter = SortAnalCounter(descArr);
                    // print
                    System.out.println(size + ", " + descCounter);
                } 
        }   
        // results of the arrays
        catch(Exception e) {
            e.printStackTrace();
        }
    }
}
