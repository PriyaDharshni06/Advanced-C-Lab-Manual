## EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

### Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
### Program:

```C
float stack[100];
int top,i;
void display()
{
    if(top==-1)
    {
        printf("stack is empty");
    }
    else
    {
         for(i=top;i>=0;i--)
         {
             printf("%.1f\n",stack[i]);
         }
    }
}
``` 

### Output:

<img width="741" height="558" alt="image" src="https://github.com/user-attachments/assets/77db3d30-776f-4985-8a97-37bceae9a543" />



### Result:
Thus, the program to display stack elements using an array is verified successfully.
 

## EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
### Aim:
To create a C program to push the given element in to a stack using array.
### Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
### Program:
```C
int size=3,top=-1;
char stack[100];
void push (char data)
{
    if (top==size-1 )
    {
    printf("stack is full\n");
    }
    else
    {
        top = top+1;
        stack[top] = data;
    }
}
``` 
### Output:

<img width="1102" height="588" alt="image" src="https://github.com/user-attachments/assets/05c87876-63c9-41a0-9798-a59ef52dfb9e" />


### Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
## EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
### Aim:
To write a C program to display queue elements using array

### Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
### Program:

```C
int front,rear;
float queue[100];
void display()
{
    if(front==-1 && rear==-1)
    {
        printf("No elements to display");
    }
    else
    {
        for(int i=front;i<=rear;i++)
        {
        printf("%.1f ",queue[i]);
        }
    }
}
``` 

### Output:

<img width="1195" height="510" alt="image" src="https://github.com/user-attachments/assets/209ab25c-5f59-4533-859e-08be6bf2b8c7" />



### Result:
Thus, the program to display queue elements using array is verified successfully.


 
## NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
### Aim:
To write a C program to insert elements in queue using array.

### Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

### Program:

```C
int size=10, rear=-1, front=-1, queue[50];
void enqueue(int data)
{
    if(rear<size)
    {
        if(front==-1)
        {
            front=0;
        }
        rear=rear+1;
        queue[rear]=data;
    }
}

``` 

### Output:
<img width="969" height="430" alt="image" src="https://github.com/user-attachments/assets/d9fcb5e5-d656-4569-9a98-842a15275e5b" />

### Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
## EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



### Aim:

To create a function in C that deletes an element from a queue implemented using an array.

### Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



### Program:

```C
int front, rear;
char queue[50];
void dequeue()
{
    if(front==-1|| front>rear)
    {
        printf("No elements to display");
    }
    else
    {
       front++;
    }
}
``` 

### Output:

<img width="1131" height="682" alt="image" src="https://github.com/user-attachments/assets/ecf63e8e-e4a1-4ff9-8bfb-7ac9f7e8a34a" />


### Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
