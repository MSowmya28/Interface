# Interface

## Aim:
To write a C# program using interface concept.

## Algorithm:
### Step 1:
Create an interface name bank.

### Step 2:
Declare 2 functions deposit() and withdraw() as abstract methods in the interface..

### Step 3:
Create a class Operations as a Child class and inherit bank.

### Step 4:
Create another class Program and inside create the Main function.

### Step 5:
Create an object for the operations class.

### Step 6:
Get Choice from user for the operation to be performed. Using switch implement the operations.

### Step 7:
Using Go-To statement you can run operations again or close the session.

### Step 8:
End of the Program.


## Program:
```
Developed By: M.Sowmya
Register Number : 212221230107
```
```
using System;
namespace Hello
{
    class Program
    {
        public interface bank
        {
            void deposit(int amount);
            void withdrwal(int amount);
        }
        public class bank1:bank
        {
            int balance = 1000;
            int amount;
            public void deposit(int amount)
            {
                balance = balance+amount;
                Console.WriteLine(balance);
            }
            public void withdrwal(int amount)
            {
                balance = balance-amount;
                Console.WriteLine(balance);
            }
            public static void Main()
            {
                bank1 obj = new bank1();
                Console.WriteLine("Enter your choice :");
                Console.WriteLine("Enter 1 to deposit");
                Console.WriteLine("Enter 2 to withdraw");
                int ch = Convert.ToInt32(Console.ReadLine());
                if (ch == 1)
                {
                    Console.WriteLine("Enter the amount to be deposited:");
                    int amount = Convert.ToInt32(Console.ReadLine());
                    Console.WriteLine("Balance Amount in your Account : ");
                    obj.deposit(amount);
                }
                else if (ch == 2)
                {
                    Console.WriteLine("Enter the amount to be withdrawed:");
                    int amount = Convert.ToInt32(Console.ReadLine());
                    Console.WriteLine("Balance Aamount in your Account : ");
                    obj.withdrwal(amount);
                }
            }
        }

    }
}

```
## Output:
![output](./c%23%209.1.png)

   
## Result:
Thus, a C# program using interface concept is written.