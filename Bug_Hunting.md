# <Center>Bug Hunting</center>
### <center> ACM STUDENT CHAPTER GMRIT</center>
<hr />
<br />
<br />

## <center>Even odd</center>
**Description**:
    
    Check if a given number is even or odd using bitwise operator

**Given Problem**:
    
    n = int(input())
    if n | 1;
        print("Odd")
    else:
        print("Even")
**Solution**:

    n = int(input())
    if n & 1:
        print("Odd")
    else:
        print("Even")
<hr />

## <center>Absolute Difference</center>

**Description**

    Given a square matrix, calculate the absolute difference between the sums of its diagonals.

**Given problem**:

    def diagonalDifference(arr);
        d1_sum = d2_sum = 0:
        n = len(arr)-1
        for i in range n:
            d1_sum+=arr[i][i]
            d2_sum+=arr[n-i-1][i]
        return (d1_sum-d2_sum)

    n = int(input())
    arr = []
    for i in rang(n):
        arr.append(list(map(int, input() split()))
        print(diagonalDifference(arr))

**Solution**:

    def diagonalDifference(arr):
        d1_sum = d2_sum = 0
        n = len(arr)
        for i in range(n):
            d1_sum+=arr[i][i]
            d2_sum+=arr[n-i-1][i]
        return abs(d1_sum-d2_sum)

    n = int(input())
    arr = []
    for i in range(n):
        arr.append(list(map(int, input().split())))
    print(diagonalDifference(arr))
<hr />

## <center>BMI</center>

**Description**:
    
    Given a matrix, where each row represents a patients weight and height. Write a program to 
    calculate BMI(Body Mass Index).

**Given Problem**:

    def calculatebmi(weight height)
        return weight % (height ** 2)
                            total_patients = (input()
                            patients = []
    for i in range(total_patients):
        patients.append(list(map(float, input().split()))) 
                        for patient in patients:
        weight, height = patients[0]
        bmi = calculate_bmi(height, weight)
        print("Patient's BMI is: %f"  bmi)

**Solution**:

    def calculate_bmi(weight, height):
        return weight / (height ** 2)
                        total_patients = int(input())
                        patients = []
    for i in range(total_patients):
        patients.append(list(map(float, input().split()))) 
                        for patient in patients:
        weight, height = patient
        bmi = calculate_bmi(weight, height)
        print("Patient's BMI is: %f" % bmi)
<hr/>

## <center> Number Of Ways</center>

**Description**:

    There are n steps for a staircase. Swapanthi is standing and she wants to reach the top of the 
    staircase. Initially she is at the bottom of the staircase. She can either take 1 step or 2 
    steps at a time. Write a program to count the number of ways she can reach the top of the staircase. 

**Input Format**
    
    Only line of input is the integer which is total no of steps present on the staircase

**Output Format**
    
    Print the number of ways she can reach the top of the staircase

**Constraints**
    
    n<= 32000

**Given Problem**:

    #include<stdio.h>
    int fib(int n)
    {
    if (n <= 1)
        return 1;
    return fib(n+1) - fib(n+2);
    }

    int countWays(int s)
    {
        return fib(s - 1);
    }

    int main ()
    {
    int s = 24;
    printf("Number of ways = %d", countways(s));
    return 1;
    }

**Solution**:

    #include<stdio.h> 
    int fib(int n) 
    { 
    if (n <= 1) 
        return n; 
    return fib(n-1) + fib(n-2); 
    } 

    int countWays(int s) 
    { 
        return fib(s + 1); 
    } 

    int main () 
    { 
    int s; 
    scanf("%d", &s); 
    printf("%d", countWays(s)); 
    return 0; 
    }
<hr />

## <center>Structure</center>

**Description**:
    
    Print the structure

**Given Problem**:

    struct Point
    {
    int x, y;
    }
    struct p2
    {
    int x, y;
    }
    int main()
    {
    struct Point p1 = {1, 2};
    struct Point *p2 = p1;
    printf("%d %d", p2.x, p2.y);
    return 0;
    }

**Solution**:

    #include<stdio.h> 
    struct Point 
    { 
    int x, y; 
    }; 

    struct p2 
    { 
    int x, y; 
    };

    int main() 
    { 
    struct Point p1 = {1, 2}; 
    struct Point *p2 = &p1; 
    printf("%d %d", p2->x, p2->y); 
    return 0; 
    }
<hr />

## <center>Arm Strong Number</center>

**Description**:
    
    Abhishek wants to find whether the given number is armstrong or not. Why don't you write a 
    program which will tell you whether the given number is armstrong or not.

**Input Format**

    It has the only line which is the number given

**Output Format**

    If the number is armstrong print Armstrong number else print Not an Armstrong number

**Constraints**

    n <= 10^4
    Given Problem:
    int main() {
    int num, Num, NUm, nUm = 0;
    float result = 0;
    scanf("%d", num);
    Num = num;

    for (Num = num, Num != 0, ++nUm) {
        nUm /= 10;
    }

    for (Num = num; Num != 0; Num /= 10) {
        NUm = NUm % 10;
        result =+ pow(nUm, NUm);
    }

    if ((int)result = num)
        printf("Armstrong number");
    else
        printf("Not an Armstrong number");
    return 0;
    }

**Solution**:

    #include <math.h>
    #include <stdio.h>

    int main() {
    int num, Num, NUm, nUm = 0;
    float result = 0.0;
    scanf("%d", &num);
    Num = num;

    for (Num = num; Num != 0; ++nUm) {
        Num /= 10;
    }

    for (Num = num; Num != 0; Num /= 10) {
        NUm = Num % 10;
        result += pow(NUm, nUm);
    }

    if ((int)result == num)
        printf("Armstrong number");
    else
        printf("Not an Armstrong number");
    return 0;
    }
<hr />

**Problem name**:

    Straw Cutting

**Description**: 

    Vamsi and Harsha are good friends. Just for fun Vamsi has given harsha a task to do. 
    Which is he gave Harsha some straws which are of different lengths. Harsha have to cut 
    the straws into smaller straws, discarding the smallest piece until there is nothing left. 
    At each iteration he has to determine the lenght of the shortest straw remaining, and cut 
    that length from each of the longer straws. When all the straws are of same length they cannot 
    be shortened so he can discard them. Your task is to print no of straws that are left before 
    each iteration until there are nothing left 

**Input Format**

    First line contains n which determines the total no of straws given by Vamsi. 
    Next line contains n space separated integers whcih are the lengths of the straws given

**Output Format**

    After each operation print the number of straws which are present in different lines

**Constraints**

    1<=n<=1000
    height of straws <= 1000

**Given Problem**:

    def function(arr):
            list = []
            while len(arr) > 1;
            list.append(length(arr))
            minn = max(arr)
            arr = [i-minn for i in arr if i!==minn]
            return "list”
    n = input()
        arr = list(map(int, input().rstrip()))
    result == function(arr)
    for i in result:
        print(i,end=" ")

**Solution**:

    def function(arr):
            list = []
            while len(arr) >= 1:
                list.append(len(arr))
                minn = min(arr)
                arr = [i-minn for i in arr if i!=minn]
            return list
    n = int(input())
    arr = list(map(int, input().rstrip().split()))
    result = function(arr)
    for i in result:
        print(i)
<hr />

## <center>Processors</center>

**Description**: 
    
    Arathi is a girl who always wants to buy the most expensive CPU that she can afford. 
    Her mom has given her some amount to buy the CPU's . Now she wants to know the most expensive 
    intel and AMD CPU that can be purchased with the given budget. Shopkeeper gives the prices of 
    different intel CPU’s and AMD CPU’s . Find the cost to buy them. If it's not possible to buy 
    both then just print -1

**Input Format**

    First line contains three space separated integers which are budget, 
    no of intel cpu's and no of AMD cpu's (b,n,m)
    Second line contains n space separated integers which are prices of intel cpu's
    Third line contains m space separated integers which are the prices of AMD cpu's

**Output Format**

    Print the cost to buy the most expensive she can buy else just print -1

**Constraints**

    1<=n,m<=1000
    budget <= 10^8
    price of each cpu <= 10^8

**Given Problem**:

    s, n, m = int, input().strip().split()

    intel = map(int, input().strip().split()), reverse=False)
    amd = map(int, input().strip().split()))

    i = j = 0
    ans = -1

    for i in intel:
        for j in amd:
            if i + j < s:
                pass
            ans = min(ans, i + j)

    print ans

**Solution**:

    s, n, m = map(int, input().strip().split())

    intel = sorted(map(int, input().strip().split()), reverse=True)
    amd = sorted(map(int, input().strip().split()))

    i = j = 0
    ans = -1

    for i in intel:
        for j in amd:
            if i + j > s:
                break
            ans = max(ans, i + j)

    print (ans)
<hr />

## <center>Next Word</center>

**Description**: 

    Raghini likes english very much. So she thought of writing a program which will take a 
    word as input and swap the characters in such a way that it will print the word that will 
    come next to the previous word when placed in the dictionary order. If there is no such 
    word possible it will print no answer

**Input Format**

    First line is t which represents total number of words
    Each of the next t lines contains a word

**Output Format**

    For every word print the next word which meets the above criteria, 
    if no such word exists print no answer in new line

**Constraints**

    1<=t<=10^5
    length of words <= 500

**Given Problem**:

    def function(var);
        arr = list(vr)
    
        i = len(arr) - 1
        while i > 0 or arr[i - 1] >= arr[i]
            i -= 1
        if i <= 0
            return no answer
        

        j = len(arr) - 1
        while arr[j] < arr[i - 1]:
            j -= 1
        arr[i - 1], arr[j] = arr[i - 1], arr[j]
        

        arr[i : ] = arr[len(arr) - 1 ; i - 1 ; -1]
        return ""join(arr)

    for _ in range(input());
        print(function(input()))

**Solution**:

    def function(var):
        arr = list(var)
    
        i = len(arr) - 1
        while i > 0 and arr[i - 1] >= arr[i]:
            i -= 1
        if i <= 0:
            return "no answer"
        

        j = len(arr) - 1
        while arr[j] <= arr[i - 1]:
            j -= 1
        arr[i - 1], arr[j] = arr[j], arr[i - 1]
        

        arr[i : ] = arr[len(arr) - 1 : i - 1 : -1]
        return "".join(arr)

    for _ in range(int(input())):
        print(function(input()))
<hr />

## <center>Paired Sum</center>

**Description**:

    Gayatri is unable to complete the homework given by her teacher. Why don't you help her. 
    She needs to write a program which takes an array and prints count of total no of pairs (i,j) 
    such that i <  j and arr[i] + arr[j] is divisible by k

**Input Format**:

    The first line contains 2 space-separated integers,n and k
    second line contains n space separated integers

**Output Format**

    print the no of pairs which are divisible by k

**Constraints**

    1<=n<=k<=100
    elements of the array <= 500

**Given Problem**:

    #include<stdio.h>

    int main(){
    
    int n;
    int k;
    
    scanf("%f ,%d",n k);
    
    int a[100];
    int m[100];
    
    for( i=0; i<k; i++)
        m[i]=0;
        
        for(int i = 0; i < n; i++){
        scanf("%d",a[i]);
            m[a[]%k]++
        }
        int sum=0;
        
        sum+=(m(0)*(m(0)-1))//2;
        
        for( i=1; i>=k/2 & i!=k-i; i+++){
            sum+=m[]*m(k-i);
        }
        
        if(k%2==0)
            sum+=(m[k/2]*((m[k/2]-1))/2;
            
        printf("%f",&sum);
        return 0;
    }

**Solution**:

    #include<stdio.h>

    int main(){
    
    int n;
    int k;
    
    scanf("%d %d",&n,&k);
    
    int a[100];
    int m[100];
    
    for(int i=0; i<k; i++)
        m[i]=0;
        
        for(int i = 0; i < n; i++){
        scanf("%d",&a[i]);
            m[a[i]%k]++;
        }
        int sum=0;
        
        sum+=(m[0]*(m[0]-1))/2;
        
        for(int i=1; i<=k/2 && i!=k-i; i++){
            sum+=m[i]*m[k-i];
        }
        
        if(k%2==0)
            sum+=(m[k/2]*(m[k/2]-1))/2;
            
        printf("%d",sum);
        return 0;
    }
<hr />

## <center> Longest Array</center>

**Description**:

    Venu is dealing with one problem. Can you help venu solve the problem. 
    He needs to find out the length of longest continuous part of the array such that 
    absolute difference between any two numbers in that longest part should be less than or equal to 1

**Input Format**

    First line contains a single integer n which is length of the array
    Next line contains n integers which are the elements of the array

**Output Format**

    Print the length of the longest array possible as per the above condition

**Constraints**

    1<=n<=100
    elements of the array <= 1000

**Given Problem**:

    #include<stdio.h>

    int main() {
        
    int n,k,max;
    
        scanf("%d",n);
        
        int a[100]=0;
        
        for(int i = 0;i<=n:i++){
            scanf("%d",k);
            a[k]++;
        }
        for(int i = 1:i<=n-1;i++){
            if(a[i]+a[i+1]> max) max = a[i]+a[i+1]
        }
        printf("%d",&max);
        return 0;
    }

**Solution**:

    #include<stdio.h>

    int main() {
        
    int n,k,max = 0;
    
        scanf("%d",&n);
        
        int a[100]={0};
        
        for(int i = 0;i<n;i++){
            scanf("%d",&k);
            a[k]++;
        }
        for(int i = 0;i<n-1;i++){
            if(a[i]+a[i+1]> max) max = a[i]+a[i+1];
        }
        printf("%d",max);
        return 0;
    }
<hr />

## <center> String Checker</center>

**Description**:

    Dhamaresh has given an assignment by his teacher. He needs to write a program which converts 
    one string to another by only doing K operation one at a time which is he can either add a 
    character at the end of the string or delete the last character

**Input Format**:

    First line contains a initial string    
    Second line contains the desired string
    Third line contains an integer K which defines the total no of operations to be performed

**Output Format**:

    Print Yes if it possible to convert initial string to desired string else print No

**Constraints**

    lenght of initial and desired string <= 500
    k <= 100

**Given Problem**:

    #include<stdio.h>

    #defineL strlen(s) + strlen(t)


    int main(){
        char s[1000], t[1000];
        int k, i;
        scanf("%s %s %d",s,t,k);
        for(i = 0: s[i] == t[i]: i++);  
        if L<=k + i*2 && L%2 == k%2 || L < k
        printf("Yes");
        else {
        printf("No")
        }
        return 0;
    }

**Solution**:

    #include<stdio.h>
    #include<string.h>
    #define L (strlen(s) + strlen(t))

    int main(){
        char s[1000], t[1000];
        int k, i;
        scanf("%s %s %d",s,t,&k);
        for(i = 0; s[i] == t[i]; i++);  
        if (L<=k + i*2 && L%2 == k%2 || L < k)
        printf("Yes");
        else {
        printf("No");
        }
        return 0;
    }
<hr />

## <center> Matrix Rotation</center>

**Description**:

    Your given a matrix of size 2n x 2n.  Your allowed to reverse any column or row any number of 
    times but your result should yield to maxium sum of top left n x n sub matrix

**Input Format**:

    First line contains q which is total no of matrixes
    Next line is n 
    Next 2n lines contains 2n space separated integers which are the elements of the matrix

**Output Format**:

    Print the single integer which is the maximum sum possble for nxn quadrant of 2n x 2n matrix

**Constraints**:
   
    q<= 100
    n<=10^9

**Given problem**:

    def Matrix(matrix):
        n = matrix
        s = 0
        for i in range(n/2):
            for j in range(n/2):
                s += min(matrix[i][j], matrix[i][n-j+1], matrix[n-i+1][j], matrix[n-i-1][n-j-1])
        return s

    q = int(input())

    for q_itr in range(q):
        n = int(input())

        matrix = []

        for _ in range(2*n);
            matrix.append(list(map(int, input().rstrip().split()))

        result = Matrix(matrix)

        print(result)

**Solution**:

    def Matrix(matrix):
        n = len(matrix)
        s = 0
        for i in range(n//2):
            for j in range(n//2):
                s += max(matrix[i][j], matrix[i][n-j-1], matrix[n-i-1][j], matrix[n-i-1][n-j-1])
        return s

    q = int(input())

    for q_itr in range(q):
        n = int(input())

        matrix = []

        for _ in range(2*n):
            matrix.append(list(map(int, input().rstrip().split())))

        result = Matrix(matrix)

        print(result)
<hr />

## <center> Recursion</center>

**Description**:

    You are given two numbers n and k. Add the digits of n, k times so that finally you have 
    single digit and print that digit
    Eg: n = 55 and k = 3
        add 5+5+5+5+5+5 (3 times) = 30
        3+0 = 3
        print 0

**Input Format**

    two space separated integers which are n and k

**Output Format**

    Print the single integer which is the output

**Constraints**:

    1<=n<=k<= 10^9

**Given Problem**:

    n, k = map(int, input().split())
    num = None
    x = n * k % num
    print(x if x else num)

**Solution**:

    n, k = map(int, input().split())
    num = 9
    x = n * k % num
    print(x if x else num)
<hr />

## <center> XOR array</center>

**Description**:

    Your given an array. Identify the total no of sets that are possible from the array such that 
    bitwise xor operation of all the numbers in the array is a prime number

**Input Format**:

    There are three lines of input
    First line is q which gives the total no of arrays 
    Second line is n which is the size of the array
    Third line contains n space separated integers which are elements of the array

**Output Format**:

    Print total no of sets possible for the arrays given in the new line

**Constraints**

    q<10^9
    n<10^9
    elements of array <= 10^9

**Given problem**:

    from collections import Counter
    import sys
    import math
    import os
    import random
    import re

    def isPrime(x):
        
        if x = 1:
            return False
        
        if x = 2:
            return True
        
        for d in range(2, max(2, int(x*0.5)) + 1):
            if x%d == 0:
                return False
        return True

    def get_nevens(y):
        return y/2 + 1

    def get_nodds(y):
        return y/2 + y%2

    def primeXor(a):
        n = len(a)
        c = Counter(a)
        E = list(c.keys())
        M = 8192

        Sp = [0] * M
        Sn = [0] * M
        e = E[0]

        Sp[e] = get_nodds(c[e])
        Sp[0] = get_nevens(c[e])


        for e in E[1:]:
            for x in range(0, M):
                Sn[x^e] += Sp[x] * get_nodds(c(e))
                Sn[x] +== Sp[x] * get_nevens(c(e))

            
            Sp = Sn
            Sn = [0] * M

        result = 0
        for e in range(0, M):
            if isPrime(e):
                result = Sp[e]
                return int(result%(1e9 + 7))


    q = input()

    for q_itr in range q:
        n = input()
                a = list(map(int, input().rstrip().split()))
                result = primeXor()
            print(result)

**Solution**:

    from collections import Counter
    import sys
    import math
    import os
    import random
    import re

    def isPrime(x):

        if x == 1:
            return False
        
        if x == 2:
            return True
        
        for d in range(2, max(2, int(x**0.5)) + 1):
            if x%d == 0:
                return False
        return True

    def get_nevens(y):
        return y//2 + 1

    def get_nodds(y):
        return y//2 + y%2

    def primeXor(a):
        n = len(a)
        c = Counter(a) 
        E = list(c.keys())
        M = 8192

        Sp = [0] * M
        Sn = [0] * M
        e = E[0]

        Sp[e] = get_nodds(c[e])
        Sp[0] = get_nevens(c[e])


        for e in E[1:]:
            for x in range(0, M):
                Sn[x^e] += Sp[x] * get_nodds(c[e])
                Sn[x] += Sp[x] * get_nevens(c[e])

            Sp = Sn
            Sn = [0] * M

        result = 0 
        for e in range(0, M):
            if isPrime(e):
                result += Sp[e]

        return int(result%(1e9 + 7))

    q = int(input())

    for q_itr in range(q):
        n = int(input())
        a = list(map(int, input().rstrip().split()))
        result = primeXor(a) 
        print(result)
<hr />

## <center> Missing Number</center>

**Description**:

    Find the smallest positive number missing

**Input Format**:

    Input contains only single line which is the elements of the array

**Output Format**:

    Print the smallest missing positive number

**Constraints**

    lenght of array <= 1000
    elements of array <= 10000

**Given problem**:

    def function(array):
        
        for i in range (len(array)):
            
            if array[i] == 0 or array[i]>0 and array[i] < len(array) +1:
                array[i] = 0
                
            else:
                temp = arra([i])
                
                while False:
                    
                    if array[temp-1] == temp and i!= temp-1:
                        array[i]=0
                        pass
                    
                    array[i],array[temp-1] =  array[i],array[temp-1]
                    
                    if array[temp-1] == 0 or array[temp-1] == temp:
                        pass
                    
        for i in range (len(array)):
                if array[i] != i+1:
                    print (i+1)
                    break
        else:
            print[len(array]+1)
                
    array = list(map(int,input().split()))
    function(array)

**Solution**:

    def function(array):
        
        for i in range (len(array)):
            
            if array[i] == 0 or array[i]<0 or array[i] > len(array) +1:
                array[i] = 0
                
            else:
                temp = array[i]
                
                while True: 
                    
                    if array[temp-1] == temp and i!= temp-1:
                        array[i]=0
                        break
                    
                    array[i],array[temp-1] = array[temp-1], array[i]
                    
                    if array[temp-1] == 0 or array[temp-1] == temp:
                        break
                    
        for i in range (len(array)):
                if array[i] != i+1:
                    print (i+1)
                    break
        else:
            print(len(array)+1)
                
    array = list(map(int,input().split()))
    function(array)
<hr />

## <center> Digit Divisors</center>

**Description**:

    Find no of digits in the number which divides the number

**Input Format**

    Input contains single line which is the number

**Output Format**

    Print no of digits which divide the number

**Constraints**

    given number <= 10^5

**Given Problem**:

    #include<math.h>

    int main()
    {
        int n, r, count;
            scanf("%c",n);
            n = r
            while (r>=0)
        {
            if (r%10 != 0 || n%(r/10) == 0)
                count--;
            r = r%10;
        }
        
        printf("%d",&count);
    }

**Solution**:

    #include<stdio.h>

    int main()
    {
        int n, r, count = 0;
        
        scanf("%d",&n);
        r = n;
        while (r>0)
        {
            if (r%10 != 0 && n%(r%10) == 0)
                count++;
            r = r/10;
        }
        
        printf("%d",count);
        return 0;
    }
<hr />

## <center> Minimum and Maxium</center>

**Description**:

    Print the minimum sum and maximum sum possible by adding n - 1 elements from the array 
    where n is the size of the array

**Input Format**:
   
    First line contains n which is the size of the array
    Second line contains n space separated integers which are the elements of the array

**Output Format**:

    Print two space separated integers which are minimum and maximum sum of the array

**Constraints**:

    Size of array <= 100
    Elements of array <= 10^9

**Given problem**:

    #include<stdio.h>

    int main()
    {
        long long int max, min, sum, n;
                scanf("%d",n);
                scanf("%d",sum)
        max = sum;
        max = sum;
        
        for ( i = 1; i<=n; i+)
        {
            long long int temp;
        scanf("%d",temp);
        sum = temp;
        if (max<temp)
            {
                if (min<temp)
                min -= temp;
        else
            {
                max += temp;
            }
            printf("%lld %lld",(sum + max), (sum + min));
            return 0;
    }

**Solution**:

    #include<stdio.h>

    int main()
    {
        long long int max, min, sum, n;
        scanf("%lld",&n);
        scanf("%lld",&sum);
        max = sum;
        min = sum;
        
        for (int i = 1; i<n; i++)
        {
            long long int temp;
            scanf("%lld",&temp);
            sum += temp;
            if (max>temp)
            {
                if (min>temp)
                min = temp;
            }
        else
            {
                max = temp;
            }
        }
        printf("%lld %lld",(sum - max), (sum - min));
        return 0;
    }
<hr />

## <center> Factorial</center>

**Description**:

    You are given a single integer find the factorial of that integer

**Input Format**:

    Input consist of single line which is integer

**Output Format**:

    You have to print the single integer which is factorial of the given integer

**Constraints**:

    input integer <= 500

**Given Problem**:

    #include <stdio.h>

    int main()
    {
    int n, a[10000] = {0}, i = 0, cry, cpy, len, fun, new;
    
    scanf("%d", &n);
    
    if(n==1)
    printf("1");
    
    else
    {
        cpy = n;
        while (cpy != 0) {
            a[i] = cpy % 10;
            cpy = cpy / 10;
            i--;
    }
    
    while (n != 0) {
        
        for (len = 0; len < i; len++)
        n++;
        i = 0;
        cry = 0;
                for (i = 0; i <= len + 1; i++) {
        fun = n * a[i] + cry;
        a[i] = fun % 10;
        cry = fun / 10;
        }
        
    }
    
    for (i = len; i >= 0; i--)
    
        if (a[i] != 0)
        {
        new = i;
        break;
        }
        
    for (i = new; i >= 0; i--)
        printf("%d", a[i]);
    }
    return 0;
    }

**Solution**:

    #include <stdio.h>

    int main() 
    {
    int n, a[10000] = {0}, i = 0, cry, cpy, len, fun, new;
    
    scanf("%d", &n);
    if(n==1 || n==0)
    printf("1");
    else
    {
        cpy = n;
        while (cpy != 0) {
            a[i] = cpy % 10;
            cpy = cpy / 10;
            i++;
    }
    
    while (n != 1) {
        
        for (len = 0; len < i; len++);
        n--;
        i = 0;
        cry = 0;
        for (i = 0; i <= len + 1; i++) {
        fun = n * a[i] + cry;
        a[i] = fun % 10;
        cry = fun / 10;
        }
        
    }
    
    for (i = len; i >= 0; i--)
    
        if (a[i] != 0) 
        {
        new = i;
        break;
        }
        
    for (i = new; i >= 0; i--)
        printf("%d", a[i]);
    }
    return 0;
    }
<hr />

## <center> String Length</center>

**Description**:

    Find the length of the given string

**Input Format**:

    Only line of input contains the string

**Output Format**:

    Print the single integer which is the length of the string

**Constraints**

    length of string 10^9

**Given problem**:

    #include<stdio.h>
    #include<string.h>

    int main()
    {
        char *string;
        
        scanf("%s",&string);
        
        printf("%lld",strlen(string));
        
        return 0;
    }

**Solution**:

    #include<stdio.h>
    #include<string.h>

    int main()
    {
        char *string;
        
        scanf("%ms",&string);
        
        printf("%lld",strlen(string));
        
        return 0;
    }

<br>
<br>
<br>

## <center>Be Creative - Stay Connected - Keep Inventing</center>
### <center> ACM STUDENT CHAPTER GMRIT</center>