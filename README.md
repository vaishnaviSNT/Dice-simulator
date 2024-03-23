# Dice-simulator
The project is a simple Python-based dice simulator that allows users to roll a six-sided dice and view the result, with an option to roll again or quit the simulation.
import random

def roll_dice():
    """
    Simulates rolling a six-sided dice.
    """
    return random.randint(1, 6)

def main():
    print("Welcome to the Dice Simulator!")
    while True:
        input("Press Enter to roll the dice (or type 'quit' to exit): ")
        result = roll_dice()
        print("You rolled:", result)
        if input("Roll again? (yes/no): ").lower() != "yes":
            print("Thanks for playing!")
            break

if __name__ == "__main__":
    main()
