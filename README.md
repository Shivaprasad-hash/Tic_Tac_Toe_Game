# Tic_Tac_Toe_Game

def game(board):
    lis = []
    for i in board:
        lis += [i]
    return lis

def checking_winner(lis_t):
    #First case 1st col ||
    if lis_t[0][0] == "O" and lis_t[1][0] == "O" and lis_t[2][0] == "O":
        print("Abhinav Wins")
    elif lis_t[0][0] == "X" and lis_t[1][0] == "X" and lis_t[2][0] == "X":
        print("Anjali Wins")
    #Second Case 1st row- -
    elif lis_t[0][0] == "O" and lis_t[0][1] == "O" and lis_t[0][2] == "O":
        print("Abhinav Wins")
    elif lis_t[0][0] == "X" and lis_t[0][1] == "X" and lis_t[0][2] == "X":
        print("Anjali Wins")
    #Third Case 2nd row- -
    elif lis_t[1][0] == "O" and lis_t[1][1] == "O" and lis_t[1][2] == "O":
        print("Abhinav Wins")
    elif lis_t[1][0] == "X" and lis_t[1][1] == "X" and lis_t[1][2] == "X":
        print("Anjali Wins")
    #Fourth Case 3rd row- -
    elif lis_t[2][0] == "O" and lis_t[2][1] == "O" and lis_t[2][2] == "O":
        print("Abhinav Wins")
    elif lis_t[2][0] == "X" and lis_t[2][1] == "X" and lis_t[2][2] == "X":
        print("Anjali Wins")
    #Fifth case 2nd col ||
    elif lis_t[0][1] == "O" and lis_t[1][1] == "O" and lis_t[2][1] == "O":
        print("Abhinav Wins")
    elif lis_t[0][1] == "X" and lis_t[1][1] == "X" and lis_t[2][1] == "X":
        print("Anjali Wins")
    #Sixth case 3rd col ||
    elif lis_t[0][2] == "O" and lis_t[1][2] == "O" and lis_t[2][2] == "O":
        print("Abhinav Wins")
    elif lis_t[0][2] == "X" and lis_t[1][2] == "X" and lis_t[2][2] == "X":
        print("Anjali Wins")
    #Seventh case diag 1
    elif lis_t[0][2] == "O" and lis_t[1][1] == "O" and lis_t[2][0] == "O":
        print("Abhinav Wins")
    elif lis_t[0][2] == "X" and lis_t[1][1] == "X" and lis_t[2][0] == "X":
        print("Anjali Wins")
    #Eighth case diag 2
    elif lis_t[0][0] == "O" and lis_t[1][1] == "O" and lis_t[2][2] == "O":
        print("Abhinav Wins")
    elif lis_t[0][0] == "X" and lis_t[1][1] == "X" and lis_t[2][2] == "X":
        print("Anjali Wins")
    else:
        print("Tie")
    
    
lis_t = []
for i in range(3):
    board = input().split()
    res = game(board)
    lis_t += [res]

checking_winner(lis_t)
