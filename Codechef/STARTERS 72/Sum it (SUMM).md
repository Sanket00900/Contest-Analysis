## Problem Link : https://www.codechef.com/problems/SUMM

Status : Scored ✅
Difficulty : Simple

Solving steps : 

1. take 3 inputs
2. check wather the sum of first two is equal to the third one

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
        
        if(a + b == c){
          System.out.println("YES");
        }else{
          System.out.println("NO");
        }
    }
  }
}
```
