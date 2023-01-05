## Problem Link : https://www.codechef.com/problems/INDIVISIBLE

States : Scored ✅ but wasteded lots of time on this silly problem 👎🏼 
Difficukty : Easy

Steps :

1. Take 3 numbers
2. Run a loop from 1 to 100
3. As soon as you find an integer that satisfies the condition, print it and break out of the loop.


## Solution : 

```
class Codechef{
	public static void main (String[] args) throws java.lang.Exception{
		Scanner s = new Scanner(System.in);
		int test = s.nextInt();
	    
    for(int t = 0; t < test; t++){
        int a = s.nextInt();
        int b = s.nextInt();
        int c = s.nextInt();
    
        for(int i = 1; i < 100; i++){
            if(a % i != 0  && b % i != 0){
                if(c % i != 0){
                    System.out.println(i);
                    break;
                  }
              }
          }
      }
   }
}
```
