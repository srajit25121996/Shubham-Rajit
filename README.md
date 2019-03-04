import java.util.Scanner;

public class Demo {

	public static boolean isPrime(int num){
		int flag=0;
		if(num==1 || num==0){
			return false;
		}
		else{
		for(int j=2;j<num;j++){
			if(num%j==0){
				return false;
			}
			
		}
		return true;
		}
			
		
		
	}
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc=new Scanner(System.in);
		
		int n= sc.nextInt();
		int m= sc.nextInt();
		int rem,temp,count;
		
		for(int i=n;i<=m;i++){
			
			temp=i;
			count=0;
			
			while(temp!=0)
			{
				rem=temp%10;
				
				if(isPrime(rem)==true){
				     count++;
		}
				temp=temp/10;
			}
			
		
		if(count==2){
					System.out.print(" "+i);
				}//if
				
			
		}	
			
			
		}//main
}//class
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
	

	


