class Person

{
	String name = null;
	int age =0;
	int Nid = 0;
	String religion = null;
	String gender = null;

	Person(String n, int a,int N,String r,String g)
	{
		name=n;
		age=a;
		Nid=N;
		religion=r;
		gender=g;
	}

void display()
	{

		System.out.println(" , Name= "+name+ ", Age= "+age+ ", Nid ="+Nid+ " , Religion= "+religion+ " , Gender= "+gender);
	}

}

class Teacher extends Person
{
    int exp=0;

	Teacher(String n, int a,int N,String r,String g, int e)

	{
		super( n, a, N, r, g);
		exp=e;
	}

void display()

{
	super.display();
	System.out.println(",Experience= "+exp);
}

}

class Student extends Person

{
   String course=null;

	Student(String n, int a,int N,String r,String g, String c)

	{
		super( n, a, N, r, g);
		course=c;
	}

void display()

{
	super.display();
	System.out.println(" COURSE="+course);
}

}

class checkMain
{
	public static void main(String args[])


	{
		Person p1= new Person("Ajgor,",24 ,20439992,"ISLAM","Male");
		p1.display();


		Teacher t1= new Teacher(" TASRINA SORKAR",30,20426221, "Islam","Female",7);
		t1.display();


		Student s1= new Student("SUDIPTO",20,2041151,"HINDU","Male","ENGLISH");
		s1.display();

	}
}
