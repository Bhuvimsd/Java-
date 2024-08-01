Remove the duplicate values
i/p:5
    1 2 1 3 2
o/p: 1 2 3

import java.util.*;
public class Main
{
   public static void main(String args[])
   {
       Scanner s=new Scanner(System.in);
       int n=s.nextInt();
       int a[]=new int[n];
       
       for(int i=0;i<n;i++)
       {
           a[i]=s.nextInt();
       }
       for(int i=0;i<n;i++)
       {
           for(int j=i+1;j<n;j++)
           {
               if(a[i]==a[j])
               {
                   for(int k=j;k<n-1;k++)
                    a[k]=a[k+1];
                   j--;
                   n--;
               }
               
           }
       }
       for(int i=0;i<n;i++)
       System.out.println(a[i]);
       
   }
}

//Write a program  to insert the value at given position in the array.

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	       int n=s.nextInt();
	       int a[]=new int[n];
	       for(int i=0;i<n;i++)
	       {
	           a[i]=s.nextInt();
	       }
	       int pos=s.nextInt();
	       int e=s.nextInt();
	       int arr[]=new int[n+1];
	       for(int i=0;i<pos-1;i++)
	       {
	           arr[i]=a[i];
	       }
	       arr[pos-1]=e;
	       for(int i=pos-1;i<n;i++)
	       {
	           arr[i+1]=a[i];
	       }
	       for(int i=0;i<n+1;i++)
	       {
	           System.out.print(arr[i]+" ");
	       }
	 }
}

pattern
ip:4
o/p:1
    **
    333
    ****
 
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int n=s.nextInt();
	    for(int i=1;i<=n;i++)
	    {
	        for(int j=1;j<=i;j++)
	        {
	            if(i%2==0)
	            {
	                System.out.print("*");
	            }
	            else{
	                System.out.print(i);
	            }
	        }
	        System.out.println();
	    }
	}
}

Largest number
ip:586
o/p:8


import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int n=s.nextInt();
	    int temp=n;
	    int max=0;
	       while(temp>0)
	       {
	           n=temp%10;
	           if(max<n)
	           {
	               max=n;
	           }
	           temp=temp/10;
	       }
	       System.out.print(max);
	    }
	}


2digits array values swap
i/p:3
    12 34 56
o/p:21 43 65

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int n=s.nextInt();
	    int a[]=new int[n];
	    for(int i=0;i<n;i++)
	    {
	        a[i]=s.nextInt();
	    }
	    for(int i=0;i<n;i++)
	    {
	        int ar=a[i]%10;
	        int b=a[i]/10;
	        int temp=ar;
	        ar=b;
	        b=temp;
	        System.out.print(b);
	        System.out.print(ar+" ");
	        
	    }
	    }
	}


i/p:a*b=9375
    a/b=15
    a+b=?


import java.util.*;
public class Main
{
  public static void main (String[]args)
  {
	Scanner s = new Scanner (System.in);
	int mul = 9375;
	int div = 15;
	int bsq = mul / div;
	int b = (int) Math.sqrt (bsq);
	int a = div * b;
	  System.out.println(a);
	 System.out.println(b);
	  System.out.print(a+b);
}
}


pattern
i/p:4
o/p:1
    3 2
    6 5 4
    10 9 8 7 


import java.util.*;
public class Main
{
  public static void main (String[]args)
  {
	Scanner s = new Scanner (System.in);
	int n=s.nextInt();
	int k=0,l=0;
	for(int i=1;i<=n;i++)
	{
	    l=k+i;
	    k=l;
	    for(int j=1;j<=i;j++)
	    {
	        System.out.print(l);
	        l--;
	    }
	    System.out.println();
	}
  }
}


Diomand pattern

import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        int n=s.nextInt();
        for(int i=1;i<=n;i++)
        {
            for(int j=1;j<=n-i;j++)
            {
                System.out.print(" ");
            }
            
            for(int k=1;k<=2*i-1;k++)
            {
                System.out.print("*");
            }
            System.out.println();
        }
        for(int i=n-1;i>0;i--)
        {
            for(int j=1;j<=n-i;j++)
            {
                System.out.print(" ");
            }
            
            for(int k=1;k<=2*i-1;k++)
            {
                System.out.print("*");
            }
            System.out.println();
        }
        
    }
        
}


import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        int n=s.nextInt();
        for(int i=1;i<=n;i++)
        {
            for(int j=1;j<=n-i;j++)
            {
                System.out.print(" ");
            }
            
            for(int k=1;k<=i;k++)
            {
                System.out.print(i+" ");
            }
            System.out.println();
        }
        
        }
        
    }

condition to make a triangle

i/p:2 0 1
o/p:No

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int a=s.nextInt();
	    int b=s.nextInt();
	    int c=s.nextInt();
	    if(a==0 || b==0 || c==0)
	    {
	        System.out.print("No");
	    }
	    
	    else if(a+b>c || a+c>b || c+b>a)
	    {
	        System.out.print("Yes");
	    }
	   

	}
}

pattern:
i/p:3
o/p:    0
      1 0 1
    2 1 0 1 2
    

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int n=s.nextInt();
	    for(int i=0;i<n;i++)
	    {
	        for(int j=n-i;j>1;j--)
	        {
	            System.out.print("  ");
	        }
	        for(int k=i;k>=0;k--)
	        {
	            System.out.print(k+" ");
	        }
	        for(int k=1;k<=i;k++)
	        {
	            System.out.print(k+" ");
	        }
	        System.out.println();
	    }
	}
}


import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int n=s.nextInt();
	    int a[]=new int[n];
	    for(int i=0;i<n;i++)
	    {
	        a[i]=s.nextInt();
	    }
	    Arrays.sort(a);
	    for(int i=0;i<n;i++)
	    {
	        int c=0;
	        for(int j=i+1;j<n;j++)
	        {
	            if(a[i]==a[j])
	           {
	               c++;
	           }
	        }
	        if(c>0)
	        {
	            System.out.print(a[i]+" ");
	        }
	    }
	}
}

Smallest even duplicate
/******************************************************************************

                            Online Java Compiler.
                Code, Compile, Run and Debug java program online.
Write your code in this editor and press "Run" button to execute it.

*******************************************************************************/
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int n=s.nextInt();
	    int a[]=new int[n];
	    for(int i=0;i<n;i++)
	    {
	        a[i]=s.nextInt();
	    }
	   int min=0;
	    for(int i=0;i<n;i++)
	    { 
	        int c=0;
	        for(int j=i+1;j<n;j++)
	        {
	               if(a[i]%2==0)
	               {
	                   if(a[i]==a[j])
	                    c++;
	               }
	                min=a[i];;
	               if(min>a[i])
	               {
	                   min=a[i];
	               }
	           }
	        }
        }
        System.out.print(min);
	}
}

if 2 power value is

ip:8
o/p:True

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int n=s.nextInt();
	    int c=0;
	    for(int i=0;i<=n;i++)
	    {
	       double p=Math.pow(2,i);
	       if(p==n)
	       {
	           c++;
	           System.out.print("True");
	           break;
	       }
        }
        if(c==0)
        {
            System.out.print("False");
        }
        
	}
}


print number till 0 if x is -ve else print till x from 0 x is +ve
i/p:-5
o/p:-5 -4 -3 -2 -1 0

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int n=s.nextInt();
	    if(n>0){
	          for(int i=0;i<=n;i++)
	          {
	            System.out.print(i+" ");
	         }
	    }
	    else if(n<0)
	    {
	        for(int i=n;i<=0;i++)
	        {
	            System.out.print(i+" ");
	        }
	    }
}
}

Gcd of two numbers
ip:12 30
op:6

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s=new Scanner(System.in);
	    int a=s.nextInt();
	    int b=s.nextInt();
	    int min=0;
	    int n=0;
	    if(a>b)
	    {
	        min=b;
	    }
	    else 
	    {
	        min=a;
	    }
	    for(int i=1;i<=min;i++)
	    {
	        if(a%i==0 && b%i==0)
	        {
	            n=i;
	        }
	    }
	    System.out.print(n);
	}
}
https://github.com/Kanishkar8844/Java.git



interface area oof circle,rectangle,triangle
import java.util.*;

interface Circle {
    void areaofc();
}

interface Rectangle {
    void areaofr();
}

interface Triangle {
    void areaoft();
}

public class Area implements Circle, Rectangle, Triangle {
    double c;  
    int c1;    
    double c2; 

    @Override
    public void areaofc() {
        int r = 5; 
    }

    @Override
    public void areaofr() {
        int l = 10; 
        int w = 5;  
        c1 = l * w;
    }

    @Override
    public void areaoft() {
        int b = 8;  
        int h = 4;  
        c2 = 0.5 * b * h;
    }

    public void display() {
        System.out.println("Area of circle: " + c);
        System.out.println("Area of rectangle: " + c1);
        System.out.println("Area of triangle: " + c2);
    }

    public static void main(String[] args) {
        Area a = new Area();
        a.areaofc();
        a.areaofr();
        a.areaoft();
        a.display();
    }
}

using interface change hight,width
import java.util.*;

interface resizable {
    void resizeWith();
    void resizeheight();
}

class rectangle implements resizable {
     int h;
     int w;
   
    public void resizeWith() {
         w=12;
    }
    
    public void resizeheight() {
        h=13;
    }
   

    public static void main(String args[]) {
       int e=100;
        rectangle r = new rectangle();
        
        r.h=e;
        r.w=e;
        System.out.println(r.h+" "+r.w); 
    }
}



import java.util.*;
interface resizable
{
    void resizewidth(int w);
    void resizeheight(int h);
}
public class Rectangle implements resizable
{
    int h;
    int w;
    public  Rectangle(int h,int w){
        this.h=h;
        this.w=w;
    }
    public void resizewidth(int w)
    {
       // this.h=h;
        this.w=w;
    }
    public void resizeheight(int h)
    {
        this.h=h;
    }
    public void display()
    {
        System.out.print("Width"+w+"Height"+h);
    }
    
	public static void main(String[] args) {
	    Rectangle r=new Rectangle(10,20);
	    r.display();
	}
}

github
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner s=new Scanner(System.in);
	int n=s.nextInt();
	for(int i=0;i<n;i++)
	{
	    for(int j=0;j<=i;j++)
	    {
	        char a=(char)(65+i);
	        System.out.print(a);
	}
	  System.out.println();
	}
}
}


import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner s=new Scanner(System.in);
	String s1=s.nextLine();
	String s2=s.nextLine();
	StringBuffer b=new StringBuffer(s2);
	String s3=b.reverse().toString();
	System.out.print(s1+s3);
}
}

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner s=new Scanner(System.in);
	String s1=s.nextLine();
	String s2=s.nextLine();
	String s3="";
    for(int i=0;i<s1.length();i++)
    {
        int c=0;
        for(int j=0;j<s2.length();j++)
        {
            if(s1.charAt(i)==s2.charAt(j))
            {
                c++;
            }
        }
        if(c<1)
        {
            System.out.print(s1.charAt(i));
        }
        
    }
}
}

ip:java
op:jaav

import java.util.*;
public class Main
{
	public static void main(String[] args) {
	Scanner s=new Scanner(System.in);
	String s1=s.nextLine();
	String s2="";
	String s3="";
    int n=s1.length()/2;
    for(int i=0;i<n;i++)
    {
        s2=s2+s1.charAt(i);
    }
    for(int i=s1.length()-1;i>=n;i--)
    {
        s3=s3+s1.charAt(i);
    }
    String s4=s2+s3;
    System.out.print(s4);
}
}

Abstract class

import java.util.*;
abstract class A
{
    public abstract void print();
    public void display()
    {
        System.out.println("zzz");
    }
}
class B extends A
{
    public void print()
    {
        System.out.println("abc");
    }
}
class Main
{
    public static void main (String[] args) {
    B b=new B();
    b.display();
    b.print();
}
}

Interface:

import java.util.*;
interface vehicle
{
    void gear(int g);
    void speed(int s);
}
class B implements vehicle
{
    int gr;
    int sp;
    public void gear(int g)
    {
        gr=g;
    }
    public void speed(int s)
    {
        sp=s;
    }
    public void print()
    {
        System.out.print(gr+" "+sp);
    }
}
class Main
{
    public static void main (String[] args) {
    B b=new B();
    b.gear(5);
    b.speed(6);
    b.print();
}
}


import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int number = scanner.nextInt();
        
        int oddPositionSum = 0;
        int evenPositionSum = 0;
        int position = 1;
        
        while (number > 0) {
            int digit = number % 10; // Extract the least significant digit
            if (position % 2 == 0) {
                evenPositionSum += digit;
            } else {
                oddPositionSum += digit;
            }
            number /= 10; // Remove the least significant digit
            position++;
        }
        
        System.out.println("Sum of digits at odd positions: " + oddPositionSum);
        System.out.println("Sum of digits at even positions: " + evenPositionSum);
        
        scanner.close();
    }
}

import java.util.*;
public class Main
{
    public static void main(String args[])
    {
        Scanner s=new Scanner(System.in);
        int n=s.nextInt();
        for(int i=1;i<=n;i++)
        {
            for(int j=i;j>=1;j--)
            {
                System.out.print(j+" ");
            }
            for(int k=2;k<=i;k++)
            {
                System.out.print(k+" ");
            }
            System.out.println();
        }
    }
}
