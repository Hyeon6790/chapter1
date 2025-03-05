### 안녕 

```
class Dog{
	String breed;
	int age;
	String color;
	
	public Dog(String breed,int age,String color) {
		this.breed = breed;
		this.age = age;
		this.color = color;
	}
	
	void barking() {
		System.out.println("barking!");
	}
	void hungry() {
		System.out.println("hungry!");
	}
	void sleeping() {
		System.out.println("sleeping!");
	}
}

public class test01{
	public static void main(String[] args) {
		Dog a = new Dog("york",1,"orange");
		System.out.println(a.breed+", "+a.age+", "+a.color);
		
		a.barking();
		a.hungry();
		a.sleeping();
	}
}
``` 
이렇게 하면 된다  
잉  
