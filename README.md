/*
 Q1) Accept age and gender from user and display the rate of interest as follow
age above 60 and gender Male (RI= 7 %)
age above 60 and gender FeMale (RI= 7.5 %)
below 60 age = RI 5%
 */
package Aaqib;
import java.util.*;
public class AgeGenderQues {
	public static void main(String [] args) {
	Scanner sc=new Scanner(System.in); // for accepting value for user
	System.out.print("Enter the age:-");
	int age=sc.nextInt();
	System.out.print("Enter the gender M for male amd F for female:-");
	char gen=sc.next().charAt(0);
	if(age>=60)
	{
		if(gen=='f' || gen=='F') // this is for male
		{
			System.out.println("Rate of intrest=7.5%");				
		}
		else {
			System.out.println("Rate of intrest=7%"); // this is for female
		}
	}
		else {
			System.out.println("Rate of intrest=5%");
		}
}
}
.....


/*
/*Q2.1) Write a program to display the following pattern
 1
   10
  101
 1010
10101
*/

package Aaqib;

public class Numpattern {

	public static void main(String[] args) {
		
		
			int i,j;
			for(i=1;i<=5;i++)  // for row
			{
				for(j=1;j<=i;j++) // for column
				{
					if(j%2==0) {
						System.out.print("0");  // if condition is true then it print
					}
					else {
						System.out.print('1'); //if condition is false then it print
					}
				
				}
				System.out.println();
			}
		}
	}

.......
 Q3.3)Write a program to display the following pattern
A
BC
DEF
GHIJ
KLMNO
 */
package Aaqib;

public class Alphabetpattern {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		char i,j;
		char ch='A'; // alphabetic patter
		for(i=1;i<=5;i++) { // for row
			for(j=1;j<=i;j++) {
				System.out.print(ch++);
			}
			System.out.println();
		}
	}

}
.....
/*
2.2 Write a program to display the following pattern 
    *         	
   ***		
  *****		
 *******		
********* 
 
 
 */
package Aaqib;

public class Starpattern {

	public static void main(String[] args) {
		//star();
		downwordstar() ;
	}
//		public static void star() {
//			int i,j;
//		for(i=1;i>=5;i++) // for row
//		{
//			for(j=1;j<=i;j++) {
//				System.out.print(" ");
//			}
//			for(j=1;j<=2*1-1;j++) //for column
//			{
//				System.out.print("*");
//			}
//			System.out.println();
//	}
//		}
//		
		/*Q3)Write a program to display the following pattern
		*********
		 *******
		  *****
		   ***
		    *
*/
		
		public static void downwordstar() {
			int x,y;
		for(x=5;x>=1;x--) // for row
		{
			for(y=5;y<=x;y++) {
				System.out.print(" ");
			}
			for(y=1;y<=x*2-1;y++) //for column
			{
				System.out.print("*");
			}
			System.out.println();
	}
	
		}
}
