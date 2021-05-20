package newpackage;

public class classanotherproject {
	protected void getname()
	{
		System.out.println("Im from another package.");
	}
}

package pack;

import newpackage.Subclassanotherproject;
import newpackage.classanotherproject;

public class Newclass {
	protected String name="Sai";
	protected void details()
	{
		System.out.println(name);
	}
}

import newpackage.Subclassanotherproject;
import newpackage.classanotherproject;
class Jala {
	public static void main(String[] args) {
		Newclass a = new Newclass();
		a.details(); // same package diff class
		classanotherproject c = new classanotherproject();
		c.getname(); //error diff package diff class
	}
}

