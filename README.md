package ex1;
import java.util.Scanner;
class Complex_Op{
	float real,imag;
    Complex_Op(){
    	 real=0;
    	 imag=0;
    }
    Complex_Op(float Comp1,float Comp2){
    	 real=Comp1;
    	 imag=Comp2;
    }
    public void AddNumber(Complex_Op C1,Complex_Op C2) {
    	float real,imag;
    	real=(C1.real+C2.real);
    	imag=(C1.imag+C1.imag);
    	System.out.println("Answer is:("+real+")+("+imag+")i");
    }
    public void SubNumber(Complex_Op C1,Complex_Op C2) {
    	float real,imag;
    	real=(C1.real-C2.real);
    	imag=(C1.imag-C1.imag);
    	System.out.println("Answer is:("+real+")+("+imag+")i");
    }
    public void MultNumber(Complex_Op C1,Complex_Op C2) {
    	float real,imag;
    	real=(C1.real*C2.real);
    	imag=(C1.imag*C1.imag);
    	System.out.println("Answer is:("+real+")+("+imag+")i");
    }
    public void DivNumber(Complex_Op C1,Complex_Op C2) {
    	float real,imag;
    	real=(C1.real/C2.real);
    	imag=(C1.imag/C1.imag);
    	System.out.println("Answer is:("+real+")+("+imag+")i");
    }
}
public class Main {

	public static void main(String[] args) {
		int ch=0;
		float num1,num2,answer;
		Complex_Op cal=new Complex_Op();
		Scanner input=new Scanner(System.in);
		System.out.println("Enter the first no.\n");
		num1=input.nextInt();
		num2=input.nextInt();
		Complex_Op Object1=new Complex_Op(num1,num2);
		System.out.println("Entre the Second Number\n");
		num1=input.nextInt();
		num2=input.nextInt();
		Complex_Op Object2=new Complex_Op(num1,num2);
		cal.AddNumber(Object1, Object2);
		cal.SubNumber(Object1, Object2);
		cal.MultNumber(Object1, Object2);
		cal.DivNumber(Object1, Object2);
	}
}
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
Output:-
Enter the first no.

1
2
Entre the Second Number

1
2
Answer is:(2.0)+(4.0)i
Answer is:(0.0)+(0.0)i
Answer is:(1.0)+(4.0)i
Answer is:(1.0)+(1.0)i
----------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------
