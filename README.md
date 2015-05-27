# JAVA-EXAMPLES
Java Programs
package calculate.factorial.using.recursion;
import java.util.Scanner; //example 1 
public class Fact {
	static int factorial(int n){
		if (n == 1){
			return 1;
		}
		else{
			return n * factorial(n-1);
		}	
	}
	public static void main(String[] args) throws Exception {
		int result;
		int number;
		String value;
			@SuppressWarnings("resource")
			Scanner scanner = new Scanner(System.in);
				System.out.println("Enter the number: ");
				value = scanner.next();
				try {
					number = Integer.parseInt(value);
					result = factorial(number);
				
					System.out.println("Factorial of " + number + " is  " +result);
					
				} catch (StackOverflowError e) {
					System.out.println("The number <= 0 "+e);
				}	
			}
	}
	

