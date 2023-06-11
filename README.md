# Java-Expt-7
# Insert an element in an Array
# Aim:
To write a Java program to insert an element in an Array.

# Algorithm
Step 1 : Open Intelli J application or any other code editor.

Step 2 : Create an array with a name of your choice.

Step 3 : Using Scanner, Input a number or a element from the user.

Step 4 : Using for loop insert the input element at the end of the array.

Step 5 : Display the append array in the terminal.

# Program

import java.util.Scanner;<br>
public class Main<br>
{<br>
    public static void main(String[] args)<br>
    {<br>
        int n, pos, x;<br>
        Scanner s = new Scanner(System.in);<br>
        System.out.print("Enter no. of elements you want in array:");<br>
        n = s.nextInt();<br>
        int a[] = new int[n+1];<br>
        System.out.println("Enter all the elements:");<br>
        for(int i = 0; i < n; i++)<br>
        {<br>
            a[i] = s.nextInt();<br>
        }<br>
        System.out.print("Enter the position where you want to insert element:");<br>
        pos = s.nextInt();<br>
        System.out.print("Enter the element you want to insert:");<br>
        x = s.nextInt();<br>
        for(int i = (n-1); i >= (pos-1); i--)<br>
        {<br>
            a[i+1] = a[i];<br>
        }<br>
        a[pos-1] = x;<br>
        System.out.print("After inserting:");<br>
        for(int i = 0; i < n; i++)<br>
        {<br>
            System.out.print(a[i]+",");<br>
        }<br>
        System.out.print(a[n]);<br>
    }<br>
}<br>
# Output:
![image](https://github.com/Anuayshh/Java-Expt-7/assets/127651217/f294f3df-64cc-47a4-99e8-f8c477755b76)


# Result
We have successfully created a Java program to Insert an element in an Array.
