# Tic Tac Toe Tutorial: 4) process what happens for that space  


## Starting state
```ruby
    # If space is available
    if space_available?(board, space)
    
      # fill in space with user icon
      # ...
      
    # If not available
    else
      # tell user not available
    end
```

## 4.1) Check if space is available
```ruby
def space_available?(board, space)
  board[space] == nil
end
```

## 4.2) Fill in space with user
```ruby
def set_space(board, space, user)
  board[space] = user
end
```


## Ending state
```ruby
if space_available?(board, space)
  set_space(board, space, current_player)
  
  # ...
else
  puts "That space is not available.  Try again"
end
```


## Full game file after this step
[Full File](/weekly_homework/tic_tac_toe/answers/4_ending_state.md)

