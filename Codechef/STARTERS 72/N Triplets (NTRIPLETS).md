## Problem Link : https://www.codechef.com/problems/NTRIPLETS

Status : Unable to solve 🚫 didnt read ps carefully, lacked in observation of hint

Imp Observation : 
1. 3 distinct positive integers A, B, C
2. Every time we can take one number as ' 1 '

## Solution : 

```
class Codechef{
	public static void main (String[] args) throws java.lang.Exception{
		Scanner s = new Scanner(System.in);
		int[]arr = new int[3];
	    int test = s.nextInt();
	    while(test-- > 0){
	        int n = s.nextInt();
	        int a = 1;
	        int b = 0;
	        int c = 0;
	        
	        for(int i = 2; i * i <= n; i++){
	            if(n % i == 0){
	                b = i;
	                c = n / i;
	                break;
	            }
	        }
	         if( a == b || b == c || c == a ){
		        System.out.println( -1 );
		    }
		    else{
		        System.out.println( a + " " + b + " " + c );
		    }
	    }
  	}
}
```
