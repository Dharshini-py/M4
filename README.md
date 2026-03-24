# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main(){
    int a,b,c;
    scanf("%d",&a);
    b=a>>2;
    c=a<<2;
    printf("After Left Shift Operation value of a is:%d\n",c);
    printf("After Right Shift Operation value of a is:%d",b);
    return 0;
}
```
<img width="973" height="538" alt="image" src="https://github.com/user-attachments/assets/3215c3c3-fe35-4c23-9297-6cf4e7961d5b" />


## OUTPUT
<img width="1052" height="331" alt="image" src="https://github.com/user-attachments/assets/ce2d76e9-25f7-4870-b037-06e41d2ff4cf" />









## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main(){
    int a,b;
    scanf("%d %d",&a,&b);
    if(a==b){
        printf("Numbers are Equal");
    }
    else{
        printf("Numbers are not Equal");
    }
    return 0;
}
```
<img width="1024" height="582" alt="image" src="https://github.com/user-attachments/assets/f3b33fa4-b607-411f-b3f2-0757839782fa" />


## OUTPUT
<img width="715" height="349" alt="image" src="https://github.com/user-attachments/assets/5cffca48-f044-4fc8-9fd7-d5e50ee5b83d" />

           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main(){
    char str[20];
    scanf("%s",str);
    for(int i=0;str[i]!='\0';i++){
        str[i]=str[i]+32;
    }
    printf("Lower case String is:%s",str);
    return 0;
}
```
<img width="727" height="606" alt="image" src="https://github.com/user-attachments/assets/2d40f4ad-fc60-4dbe-8377-3c77ee76076b" />


## OUTPUT
<img width="817" height="301" alt="image" src="https://github.com/user-attachments/assets/f911eedd-5bfa-4d3b-96f5-4a0f817e55b9" />




## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main(){
    char str[100];
    int i=0,words=1;
    scanf("%[^\n]s",str);
    do{
        if(str[i]==' '){
            words++;
        }
        i++;
    }while(str[i]!='\0');
    printf("%d\n",words);
    return 0;
}
```
<img width="971" height="678" alt="image" src="https://github.com/user-attachments/assets/0c4ad8ed-f3ab-4685-bde5-a510acd3738a" />


## OUTPUT

<img width="572" height="299" alt="image" src="https://github.com/user-attachments/assets/cf388bbe-7d7a-498c-8ca5-7818fee751fa" />




## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
    char str1[100], str2[100];
    int i = 0, flag = 0;
    scanf("%s", str1);
    scanf("%s", str2);
    while(str1[i] != '\0' || str2[i] != '\0')
    {
        if(str1[i] != str2[i])
        {
            flag = 1;
            break;
        }
        i++;
    }
    if(flag == 0)
        printf("strings are same");
    else
        printf("strings are not same");
    return 0;
}
```
<img width="640" height="768" alt="image" src="https://github.com/user-attachments/assets/ddf0e9d7-f4ca-4230-9e6f-b602700cdb8b" />


## OUTPUT
<img width="693" height="345" alt="image" src="https://github.com/user-attachments/assets/87c5ae07-132e-4e87-b63a-5ca41284b1c8" />


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

