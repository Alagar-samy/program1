# program1
Hello mam. Here I'm using python for the program
step1: Store the given input in a list and assign a variable 'count' as 1.
step2: Put a for loop which starts with 0 upto n.
step3: Then put an if condition(a[i]!=' ').If it is true then it goes to step 4.
step4: Create an inner loop and it starts with i+1 upto n.
step4: Put an if condition(a[i]==a[j]). If it is true then the count value will increments and assign ' ' to a[j].
step6: After the inner loop gets stopped, print the count value and assign count to 0.

here is the code for the given program

count=1
a=list(input("enter the string"))
n=len(a)
for i in range(0,n):
    if(a[i]!=" "):
        for j in range(i+1,n):
            if(a[i]==a[j]):
                count+=1
                a[j]=" "
        print(a[i],count)
        count=1
