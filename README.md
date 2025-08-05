Art Dice Roller
A fun and simple command-line Python script that simulates rolling multiple six-sided dice. It displays the results using beautifully rendered ASCII art and calculates the total sum of the roll.

Preview:
When you run the script and ask for 3 dice, the output will look something like this:
<img width="1303" height="320" alt="image" src="https://github.com/user-attachments/assets/6b9c7e8d-ac36-4745-9f99-0e17d0583cf6" />

Features:
Dynamic Number of Dice: You can specify how many dice you want to roll each time you run the script.
ASCII Art Display: Each die roll is represented visually with a unique ASCII art face, from 1 to 6.
Horizontal Layout: The dice are printed side-by-side for a clean, organized view.
Total Sum Calculation: The script automatically calculates and displays the sum of all dice rolled.
Lightweight & Simple: No external libraries are needed—it runs with standard Python.

How to Use:
To run this script, you just need Python 3 installed on your system.
Save the code: Save the code into a file named dice_roller.py.
Run from the terminal: Open your terminal or command prompt, navigate to the directory where you saved the file, and run the following command:
python dice_roller.py
Enter the number of dice: The script will then prompt you to enter how many dice you want to roll. Type a number and press Enter to see the results!

How It Works:
The script's logic is straightforward:
dice_art Dictionary: A dictionary stores the ASCII art for each of the 6 possible faces of a die. The key is the integer (1-6), and the value is a tuple of strings, where each string is a line of the drawing.
User Input: The script asks the user for the number of dice to simulate.
Rolling the Dice: A for loop runs as many times as the number of dice requested. In each iteration, it generates a random integer between 1 and 6 and appends it to a dice list.
Printing the Art: To print the dice horizontally, the code iterates through each line of the ASCII art (from 0 to 4). In an inner loop, it prints the corresponding line for each die that was rolled, using end=" " to prevent newlines. After printing a full line for all dice, it moves to the next line.
Calculating the Total: Finally, it loops through the dice list one more time to sum up the values and prints the total to the console.
