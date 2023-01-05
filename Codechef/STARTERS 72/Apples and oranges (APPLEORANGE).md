## Problem Link : https://www.codechef.com/problems/APPLEORANGE

Status : Solved ✅ observed well 👍🏼

Difficulty : easy

Observsation : 

1. k must be a divisor of NN and a divisor of MM.
2. The largest such kk is, by definition, gcd(N, M) or gcd(N,M); and this is the answer.

#### Challenge : Constrains ->     1 <= N , M <= 10^9 

Best way to find GCD of two numbers =>  Euclidean algorithm (https://cp-algorithms.com/algebra/euclid-algorithm.html) 


## Solution :

```
class Codechef{
	public static void main (String[] args) throws java.lang.Exception{
		Scanner s = new Scanner(System.in);
		int test = s.nextInt();
	    for(int t = 0; t < test; t++){
            long a = s.nextInt();
            long b = s.nextInt();
        
	        long ans = GCD(a,b);
	        System.out.println(ans);
        }  
	}
	
	private static long GCD(long a, long b) {
        if (a == 0)
           return b;
        else if (b == 0)
           return a;
        else if (a == b)
            return a;

        if (a > b)
            return GCD(a-b, b);
        return GCD(a, b-a);
    }
}
```
