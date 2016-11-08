## Review 

In preparation for your test tomorrow, take the time to step through the code line by line and reproduce the output. 

The problem sets are pencil-and-paper exercises rather than programming problems, but feel free to use the computer to check your work. You won't have a computer for the test so it is important to make sure that you can solve them without electronic assistance


 **Problem 1**
```
    public static void main(String[] args) {
        bludger(2001);
    }

    private static void bludger(int y) {
        int x = y / 1000;
        int z = (x + y);
        x = quaffle(z, y);
        System.out.println("bludger: x = " + x + ", y = " + y + ", z = " + z);
    }

    private static int  quaffle(int x, int y) {
        int z = snitch(x + y, y);
        y /= z;
        System.out.println("quaffle: x = " + x + ", y = " + y + ", z = " + z);
        return z;
    }

    private static int snitch(int x, int y) {
        y = x / (x % 10);
        System.out.println("snitch: x = " + x + ", y = " + y);
        return y;
    }
```

 **Problem 2**
```
  public static void main(String[] args) {
        ghost(13);
    }

    private static void ghost(int x) {
        int y = 0;
        for (int i = 1; i < x; i *= 2) {
            y = witch(y, skeleton(x, i));
        }
        System.out.println("ghost: x = " + x + ", y = " + y);
    }

    private static  int witch(int x, int y) {
        x = 10 * x + y;
        System.out.println("witch: x = " + x + ", y = " + y);
        return x;
    }

    private static int skeleton(int x, int y) {
        return x / y % 2;
    }
```
 **Problem 3**
```
  public static void main(String[] args) {
        String s1 = "Heart";
        String s2 = valentine("candy", s1);
        System.out.println("s1 = " + s1);
        System.out.println("s2 = " + s2);
    }

    private static String valentine(String s1, String s2) {
        int num = (s1.substring(1, 2)).length();
        s1 = s2.substring(num);
        s2 = cupid(s1, s2.charAt(0));
        return (s2);
    }

    private static String cupid(String s1, char ch) {
        return (s1 + Character.toLowerCase(ch));
    }
```
 **Problem 4**

What is the value of `mystery(1729)`?

```
 private int mystery(int n) {
        while (n >= 10) {
            int k = 0;
            while (n > 0) {
                k += n % 10;
                n /= 10;
            }
            n = k;
        }
        return n;
    }
```


 **Problem 5**

```
for(int i = 0; i < 3; i++) 
{ 
    switch(i) 
    { 
        case 0: break; 
        case 1: System.out.print("one "); 
        case 2: System.out.print("two "); 
        case 3: System.out.print("three "); 
    } 
} 
System.out.println("done");
```

**Problem 6**

Review this code and run through it to the best of your ability: 

https://accesscode3-3.slack.com/files/jsjrobotics/F2XNM7CV6/statemachine.java
