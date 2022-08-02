# What is Random Sentence Generator (Note: A React app with a custom API is being developed on Heroku. I have included only a conceptual clean java code here.)


### Basic Random Sentence Generator from Your Own Data Set -
#### The purpose of this code is for beginners who want to keep motivated to code by making their own dataset and adding sentences on a regular basis as well as increase the stock of sentences.

Note: 
* You should update your database once a day using online IDE, and you should run the program daily to refresh your stock of data 
  * [Online IDE](https://www.programiz.com/java-programming/online-compiler/) 
* Adding and memorizing one sentence every day gives you the ability to learn 365 sentences in a year if you double or triple it, it will increase your stock of sentences by twice or three times. 

## In JAVA (Structure of the code is given below) - Clean Code

```java
import java.util.Random;
// basic random sentence generator in from  your own data set
public class CodeXam {

//========================================================================================================================================================
    /*
       RULE 0:  ADD MOVIE NAME WITH LINE AND MEANING OF THE LINE

      RULE 1 : Replicate LAST Line from DATA SET - THEN CHANGE THE LINE NUMBER(STRING REFERENCE) TO MATCH THE DATA SET AND ADD YOUR DATA ON THIS STRING

      RULE 2 : Replicate LAST Line from OPERATE FUNCTION - THEN REPLACE THE NEXT NUMBER IN CASE FUNCTION AND CHANGE THE LINE NO(STRING REFERENCE)
     * */
//=======================================================================================================================================================

    // DATA ADD WITH COUNTING - DATA SET
    public static void main(String[] args) {

        int row_increase = 0;
        String line1 = "The quick brown fox jumps over the lazy dog";
        String meaning1 = "A sentence";
        row_increase++;


        String line2 = "The quick brown fox jumps over the lazy dog 2";
        String meaning2 = "A sentence 2";
        row_increase++;


        String line3 = "The quick brown fox jumps over the lazy dog 3";
        String meaning3 = "A sentence 3";
        row_increase++;



        //______________________________________________________________________________________________________________________________
        //______________________________________________________________________________________________________________________________



        //PRINTING TOTAL DATASET
        System.out.println("Total Dataset Added: " + row_increase);


        //______________________________________________________________________________________________________________________________
        //______________________________________________________________________________________________________________________________




        //ADDING DATASET TO RANDOM FUNCTION - OPERATE FUNCTION
        Random rd = new Random();//random dataset of grammar line
        int comp_input = rd.nextInt(row_increase); //taking input from the computer

        switch (comp_input) {
            case 0: { // if our random program generate zero
                System.out.println(comp_input + " No Line. " + line1 + "\n" + "Hinglish meaning of this line  : " + meaning1);
            }
            break;


            case 1: { // if our random program generate one
                System.out.println(comp_input + " No Line. " + line2 + "\n" + "Hinglish meaning of this line  : " + meaning2);
            }
            break;


            case 2: { // if our random program generate two
                System.out.println(comp_input + " No Line. " + line3 + "\n" + "Hinglish meaning of this line  : " + meaning3);
            }
            break;
       }
    }
}


```





