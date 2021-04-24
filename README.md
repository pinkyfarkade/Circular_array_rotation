import java.util.*;
class Solution
{
    public static void main(String gg[])
    {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int k=sc.nextInt();
        int q=sc.nextInt();
        int arr[]=new int[n];
        for(int i=0;i<n;i++)
        {
            arr[i]=sc.nextInt();
        }
     
        for(int j=0;j<k;j++)
        { 
            int a=arr[n-1];
            for(int i=n-1;i>0;i--)
            {
                
                arr[i]=arr[i-1];
                
            }
             arr[0]=a;
        }
       
        for(int i=0;i<q;i++)
        {
            int arr1=sc.nextInt();
            System.out.println(arr[arr1]);
        }
    
    }
}
 
