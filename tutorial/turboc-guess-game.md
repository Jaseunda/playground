**Instructions:**

1. **Open your Turbo C++ IDE:** Start by opening your Turbo C++ IDE. Create a new file for your program.

2. **Start your program:** Include necessary headers and start your main function.

```cpp
#include<iostream.h>
#include<conio.h>
#include<stdlib.h>

void main()
{
   // your code here
}
```

3. **Initialize necessary variables:** Declare the variables that you'll use in your program. For this game, you'll need the target number, the player's guess, and the number of attempts.

```cpp
void main()
{
   int target, guess, attempts = 0;
   // your code here
}
```

4. **Generate a random target number:** For this, you'll use the rand() function and modulus operator to limit the range of the target number (e.g., from 1 to 100).

```cpp
void main()
{
   int target, guess, attempts = 0;
   target = rand() % 100 + 1;  // generates a random number between 1 and 100
   // your code here
}
```

5. **Start the game loop:** Create a while loop for the player to keep guessing until they get the correct answer.

```cpp
void main()
{
   int target, guess, attempts = 0;
   target = rand() % 100 + 1;  

   while(1)  // game loop
   {
      // your code here
   }
}
```

6. **Get player's guess:** Inside the loop, prompt the player to enter their guess and use cin to get the input.

```cpp
while(1)  // game loop
{
   cout << "Enter your guess: ";
   cin >> guess;
   attempts++;
   // your code here
}
```

7. **Check the guess:** Use if-else statements to check if the guess is higher, lower, or equal to the target number. If the guess is correct, break the loop.

```cpp
while(1)  // game loop
{
   cout << "Enter your guess: ";
   cin >> guess;
   attempts++;

   if(guess < target)
   {
      cout << "Too low!\n";
   }
   else if(guess > target)
   {
      cout << "Too high!\n";
   }
   else
   {
      cout << "Correct! You've guessed the number in " << attempts << " attempts.\n";
      break;
   }
}
```

8. **End your program:** Close your main function and run your program.

```cpp
void main()
{
   int target, guess, attempts = 0;
   target = rand() % 100 + 1;  

   while(1)  // game loop
   {
      cout << "Enter your guess: ";
      cin >> guess;
      attempts++;

      if(guess < target)
      {
         cout << "Too low!\n";
      }
      else if(guess > target)
      {
         cout << "Too high!\n";
      }
      else
      {
         cout << "Correct! You've guessed the number in " << attempts << " attempts.\n";
         break;
      }
   }
   getch();
}
```

