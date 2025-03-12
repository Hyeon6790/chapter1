```
package chapter01;
class Member{//상위 클래스
	String name;//속성
	int age;
	String tel;
	String email;
	
	public Member(String name,int age,String tel,String email) {//메소드
		this.name = name;
		this.age = age;
		this.tel = tel;
		this.email = email;
		
	}
	public void printMsg() {
		System.out.println("이름 : "+name);
		System.out.println("나이 : "+age);
		System.out.println("전화번호 : "+tel);
		System.out.println("이메일 : "+email);
		
		
	}
}
class Studente extends Member{ //상속 하위 클래스
	int score;
	
	public Studente(String name,int age,String tel,String email,int score) {
		super(name,age,tel,email);//상위 클래스 생성자를 호출하는 방법
		this.score = score;
	}
	public void printMsg() {
		super.printMsg();
		System.out.println("점수 : "+score);
	}
}

public class Task03 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Studente a = new Studente("홍길동",25,"010-111-1111","hong@naver.com",85);
		a.printMsg();
	}

}


```
