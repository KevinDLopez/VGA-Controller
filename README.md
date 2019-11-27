# VGA-Controller
Animated VGA 
	In this project I modified my previous progress to make the ball and the paddle so that they could move. 
  I added a register for the lower portion of the paddle so that when someone holds down the up/down button 
  the paddle would move in such direction. For the upper portion of the paddle I just did the register – 72. 
  Seventy-two being the length of the paddle.  When it would reach the bottom or top the paddle won’t be moving. 
  For the ball I used a Y and X position registers. And just added eight for the other side of the ball.
  We made the ball move by having a position change register, one on X and one on Y.  
    I made all this change to happen at 60hz which the actual refresh rate of the monitor is. 
  I had an error where the ball wouldn’t change
  to negative when getting to the walls or paddles, this was caused because I was using a three-bit reg and when
  I try to change it to a negative number the change won’t happen since there is more bits to represent a 
  negative number.  I solved this by changing such reg to ten bits wide which is enough for representing negative four.
  
  
  # Top Level Block Diagram
![Detail Level block Diagram](https://camo.githubusercontent.com/bcb02353a16ac556b37567b8135a27514cff276d/687474703a2f2f692e696d6775722e636f6d2f66716174632e706e67)


