```
package Chapter01;

import java.util.Scanner;

class PlusMinus{
	//속성
	int plus;
	int minus;
	
	String plus(int x, int y) {
		this.plus = x + y;
		return "두 값의 덧셈 : "+ this.plus;
	}
	
	String minus(int x,int y) {
		this.minus = x - y;
		return "두 값의 뺄셈 : "+ this.minus;
	}
}

class MultiDiv extends PlusMinus{// 상속 = extends 단일 상속만 허용한다.
	
	int multi;
	double div;
	
	String multi(int x,int y) {
		multi = x * y;
		return "두 수의 곱셈 : " + multi;
	}
	String div(int x,int y) {
		div = x / y;
		return "두 수의 나눗셈 : " + div;
	}
	
	
}

public class Test02 {

	public static void main(String[] args) {
		
		//PlusMinus get = new PlusMinus();//()값을 아무것도 넣으면 0값으로 초기화 =자동생성자 메소드
		
	/*	String minus = get.minus(10,20);
		System.out.println(minus);
		
		String plus = get.plus(10,20);
		
		System.out.println(plus);*/
		//---------------------------------------------------------------------------//
		/*
		Scanner data = new Scanner(System.in);//키보드 입력 Scanner = new Scanner(System.in)
		
		System.out.println("x 값: ");
		int x = data.nextInt();//정수 = .nextInt 문자nextLine
		System.out.println("y 값: ");
		int y = data.nextInt();
		PlusMinus get = new PlusMinus();
		String plus =get.plus(x,y);
		System.out.println(plus);
		*/
		//------------------------------------------------------------------------------//
		MultiDiv cal = new MultiDiv();
		System.out.println(cal.plus(20,10)); 
		System.out.println(cal.minus(20,10)); 
		System.out.println(cal.multi(20,10)); 
		System.out.println(cal.div(20,10)); 
		}
}
```
