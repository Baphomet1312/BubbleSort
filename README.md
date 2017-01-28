# BubbleSort


package lesson12;

import java.util.Arrays;

public class BubbleSort2 {

	public static void main(String[] args) {
		int [] myArray = {15,39,22,4,5,6,1,10,1,0};
		
		int last = myArray[myArray.length - 1];
		int prelast = myArray[myArray.length - 2];
		
		if(myArray[prelast] > myArray[last]) {
			
			int temp = myArray[prelast];
			
			myArray[prelast] = myArray[last];
			myArray[last] = temp;
 		}
		for (int i = myArray.length - 1; i >= 0;i--) {
            for (int b = 0; b < i; b++) {
            	if( myArray[b] > myArray[b+1] ){
                    int temp = myArray[b];
                    myArray[b] = myArray[b+1];
                    myArray[b+1] = temp;
                    
                   

}}
            System.out.println(Arrays.toString(myArray)); 
	
		}
}}
