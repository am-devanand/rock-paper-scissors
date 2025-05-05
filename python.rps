import random

def get_user_choice():
    choice = input("Enter Rock, Paper, or Scissors: ").strip().lower()
    if choice in ['rock', 'paper', 'scissors']:
        return choice
    else:
        print("Invalid input. Try again.")
        return get_user_choice()

def get_computer_choice():
    return random.choice(['rock', 'paper', 'scissors'])

def determine_winner(user, computer):
    if user == computer:
        return "It's a tie!"
    elif (
        (user == 'rock' and computer == 'scissors') or
        (user == 'paper' and computer == 'rock') or
        (user == 'scissors' and computer == 'paper')
    ):
        return "You win!"
    else:
        return "Computer wins!"

def play():
    print("=== Rock, Paper, Scissors Game ===")
    user_choice = get_user_choice()
    computer_choice = get_computer_choice()
    print(f"\nYou chose: {user_choice.capitalize()}")
    print(f"Computer chose: {computer_choice.capitalize()}")
    result = determine_winner(user_choice, computer_choice)
    print(f"\nResult: {result}")

if __name__ == "__main__":
    play()
