# Java-
Program Strong Number


import java.util.Scanner;
	public class PracticeClass2
	{
		public static void main(String[]args)
		{
			int ino,digit=0,temp,sum=0,f;
			Scanner obj=new Scanner(System.in);
			System.out.println("Enter any number to check strong or not strong");
			ino=obj.nextInt();
			temp=ino;
			while(temp!=0)
			{
				f=1;
				digit=temp%10;
			while(digit>=1)
			{
				f=f*digit;
				digit++;
			}
			sum=sum+f;
			temp/=10;
		}
		if(ino==sum)
		System.out.println("Its strong number");
		else
		System.out.println("Its not strong number");
	}
}
