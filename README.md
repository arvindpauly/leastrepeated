# leastrepeated
import java.util.ArrayList;
import java.util.Arrays;
import java.util.Collections;
import java.util.Scanner;

public class RepeatedString {
	public static void main(String[] args) {
		int num;
		Scanner ab = new Scanner(System.in);
		System.out.println("enter the number of terms");
		num = ab.nextInt();
		System.out.println("enter the numbers");
		int[] array = new int[num];
		for (int i = 0; i < array.length; i++) {
			array[i] = ab.nextInt();
			

		}ArrayList<Integer>a=new ArrayList<Integer>();
		int k=0;
		int count=0;
		for (int i = 0; i < array.length-1; i++) {
			for (int j = i; j < array.length-1; j++) {
				
			
			
				if(array[i]==array[j])
				{
					a.add(array[i]);
					count++;
				}
				
			}
		}
		Collections.sort(a);
		if(count>0)
		{
			System.out.println("the least repeated value"+a.get(0));
		}
		else
		{
			System.out.println("there is no any  reapted values ");
		}

	}
}
