import java.lang.String;
import java.util.Scanner;
public class CamelCase
{
  public static void main(String args[])
  {
    Scanner sc=new Scanner(System.in);
    System.out.println("ENTER A STRING:");
    String str=sc.nextLine();
    Char arr[]=str.toCharArray();
    arr[0]=arr[0].toUpperCase();
    for(int i=0;i<arr.length;i++)
    {
      if(arr[i]==' ')
           arr[i+1]=arr[i+1].toUpperCase();
     }
     for(int j=0;j<arr.length;j++)
     System.out.println("CAMEL CASE:"+arr[j]);
    }
   }
