import java.util.Scanner;
import java.lang.Math;

class Student
{
double subjectMarks[]= new double[10];
double credits[]= new double[10];
double grade[]=new double[10];
String name;
String usn;
double SGPA;

void getStudentDetails()
{
Scanner s = new Scanner(System.in);
System.out.print("Enter your Name: ");
name = s.next();
System.out.print("Enter your USN: ");
usn = s.next();
}

double getMarks()
{
Scanner s = new Scanner(System.in);
int i;
double effectiveScore=0;
double totalCredits = 0;
double SGPA;

for(i=1;i<=3;i++)
{
System.out.print("Enter marks for subject "+(i)+" : ");
subjectMarks[i] = s.nextInt();
System.out.print("Enter credits for subject "+(i)+" : ");
credits[i] = s.nextInt();

grade[i] = ((subjectMarks[i])/10);
grade[i]=Math.floor(grade[i]+1);
if(grade[i]<4)
{
grade[i] = 0;
}
effectiveScore = effectiveScore + (grade[i]*credits[i]);
totalCredits = totalCredits + credits[i];
}
SGPA = effectiveScore/totalCredits;
return SGPA;

}  
}

class Main
{
public static void main(String args[])
{
int i,n;
double value;
Scanner s= new Scanner(System.in);
System.out.println("Enter number of students:");
n=s.nextInt();
for (i=0;i<n;i++){
Student s1 = new Student();
s1.getStudentDetails();
value=s1.getMarks();
System.out.println("Name: "+s1.name);
System.out.println("USN: "+s1.usn);
System.out.println("SGPA: "+value);
}
}
}
