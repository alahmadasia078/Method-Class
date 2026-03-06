```csharp
using System; // Import core namespace for Console

// Define a custom class
public class MathOperations
{
    // Void method that takes two integers as parameters
    public void ProcessNumbers(int firstNumber, int secondNumber)
    {
        // Do a math operation on the first integer (example: multiply by 2)
        int result = firstNumber * 2;

        // Display the math result for the first integer
        Console.WriteLine("The first number doubled is: " + result);

        // Display the second integer directly
        Console.WriteLine("The second number provided is: " + secondNumber);
    }
}

class Program
{
    static void Main(string[] args)
    {
        // Instantiate the MathOperations class
        MathOperations mathOps = new MathOperations();

        // Call the method, passing in parameters by position
        mathOps.ProcessNumbers(5, 10); 
        // Explanation: firstNumber = 5, secondNumber = 10 → output is doubled first number and raw second number

        // Call the method, passing in parameters by name
        mathOps.ProcessNumbers(secondNumber: 20, firstNumber: 7);
        // Explanation: firstNumber = 7, secondNumber = 20 → demonstrates named parameters usage

        // Pause the program so the console stays open (for viewing results)
        Console.ReadLine();
    }
}
```

---

### **Step-by-Step Explanation**
1. **`MathOperations` class** → Holds a method called `ProcessNumbers`.
2. **`ProcessNumbers` method** → Accepts two integers, performs a math calculation on the first, prints both to the console.
3. **Instantiate class** → Done in `Main()` using `new`.
4. **Call method: positional parameters** → `mathOps.ProcessNumbers(5, 10)`.
5. **Call method: named parameters** → `mathOps.ProcessNumbers(secondNumber: 20, firstNumber: 7)`.
6. **Comments** → Added above each step to make it clear for other developers.