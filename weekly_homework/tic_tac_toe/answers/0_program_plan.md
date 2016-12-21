# Tic Tac Toe Tutorial: Program Plan

## Main structure of program

```ruby
def start_game

  # 1. Create starting state of board

  # Create user list
  users = ['X', 'O']  

  # Choose first player
  current_player = users.first

  # Create initial conditions for while loop
  game_over = false
  while game_over != true

    # 2. Print out current game board

    # 3. Get user input (a space number)

    # 4. Process what happens for that space
    # If space is available
      # fill in space with user icon

      # 5. Check if game over, by win or tie
      # 6. if game over
        # Tell user what happened
        # Terminate the loop
      # 7. if not over
        # change to other user
    # If not available
      # tell user not available
  end
end

start_game
```

## List of pieces and explanations
Plug each of these pieces into the structure above

  
### 1. Create starting state of board  
For the first example, we will use a single 9 space array.  

```ruby
board = [nil, nil, nil, nil, nil, nil, nil, nil, nil]

# Shortcut
board = [nil] * 9
```

### 2. Print out current game board  
```ruby
# To call function in the while loop
print_game_board(board)

# Structure of function
def print_game_board(board)
  # print first row of spaces
  # print divider
  # print second row of spaces
  # print divider
  # print third row of spaces
end
```
  
[Answer](2_print_game_board.md#tic-tac-toe-tutorial-2-print-game-board)


### 3. Get user input (a space number)  
This assumes that the user will enter a number in range of the board

```ruby
user_input = gets.chomp.to_i
```

#### Optional
1) Check that user entered a number 0-8  
2) Add ability for user to exit the game  

### 4. process what happens for chosen space  
```ruby
if space_available?(board, space)
  # fill in space with user icon
  # ...
# If not available
else
  # tell user not available
end
```

[Answer](4_process_space_choice.md)

### 5. check if game over  
  - check for win  
  - check for tie  

### 6. handle game over case
  - Tell user what happened  
  - Terminate the loop  

### 7. handle game continue case    
  - change to other user    


