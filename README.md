import java.lang.String;
import java.util.Scanner;
public class CamelCase
{
  public static void main(String args[])
  {
    Scanner sc=new Scanner(System.in);
    String str=sc.nextLine();
    char arr[]=str.toCharArray();
    for(int j=0;j<arr.length;j++)
    {
    if(Character.isLetter(arr[j]))
      count++;
     }
     if(count==arr.length-1)
     {
    arr[0]=Character.toUpperCase(arr[0]);
    for(int i=0;i<arr.length;i++)
    {
      if(arr[i]==' ')
           arr[i+1]=Character.toUpperCase(arr[i+1]);
     }
     System.out.println("CAMEL CASE:");
     for(int j=0;j<arr.length;j++)
     System.out.print(arr[j]);
    }
    else
      System.out.println("0");
    }
   }
