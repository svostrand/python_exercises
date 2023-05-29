import random

def print_score():
    print('The Final Score:')
    print(f'Player 1: {player1_score}')
    print(f'Player 2: {player2_score}')
    print(f'Total Draws {draws}')
  
player1_score = 0
player2_score = 0
draws = 0

choices = ['rock', 'paper', 'scissors', 'rock', 'paper', 'scissors']
x = 0
while x < 1000:
    x = x + 1
    player_1 = random.choice(choices)
    player_2 = random.choice(choices)

    match player_1:
        case 'rock':
            if player_2 == 'rock': draws = draws + 1
            elif player_2 == 'scissors': player1_score = player1_score + 1
            elif player_2 == 'paper': player2_score = player2_score + 1
        case 'paper':
            if player_2 == 'paper':  draws = draws + 1
            elif player_2 == 'scissors': player2_score = player2_score + 1
            elif player_2 == 'rock': player1_score = player1_score + 1
        case 'scissors':
            if player_2 == 'scissors':  draws = draws + 1
            elif player_2 == 'rock': player2_score = player2_score + 1
            elif player_2 == 'paper': player1_score = player1_score + 1
        case _: print('unknown')

if player1_score == player2_score:
    print('its a draw')
    print_score()
elif player1_score > player2_score:
    print('Player 1 wins')
    print_score()
else:
    print('Player2 wins')
    print_score()
