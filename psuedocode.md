# Scratch Project

## Ball
When 'Flag' Clicked
* Forever
  * Move 5 steps towards cursor

When 'Flag' Clicked
* Show ball
* Switch to blue ball
* Forever
  * Wait one second
  * Change Score by 1

When 'Flag' Clicked
* Forever
  * If touching the square
    * Then broadcast 'Game Over'

When I receive 'Game Over'
* If my score is greater than my high score
  * Then set my high score to be equal to that score
* Set score back to zero
* Hide ball
* Stop all threads

When I receive 'Speed'
* Loop 50 times
  * Move 7 steps towards cursor
  * Switch costume every .1 seconds
  
## Square
When 'Flag' Clicked
* Print
* Set size to 100%
* Forever
  * Glide a random time 1-5 seconds to a random location on the screen

When 'Flag' Clicked
* Forever
  * If your score is greater then 50
    * Then increase size .5
    
When I receive 'Game Over'
* Hide

## Arrow
When 'Flag' Clicked
* Hide
* Wait 10 seconds
* Show
* Forever
  * Glide a random time 1-5 seconds until you reach the edge, turn 180 degrees and repeat
  
When I receive 'Game Over'
* Hide
* Go to original spot

When 'Flag' Clicked
* Forever
  * If touching the ball
    * Then broadcast 'Game Over'
   
## Apple
When 'Flag' Clicked
* Hide
* Forever
  * Pick a random time 1-5 seconds
  * Show
  * Go to a random position on the screen

When 'Flag' Clicked
* Forever
  * If touching the ball
    * Then broadcast '2x'
    
When I receive '2x'
* Hide
* Add 5 to total score

When I receive 'Game Over'
* Hide

## Golden Apple
When 'Flag' Clicked
* Forever
  * If touching the ball
    * Then broadcast 'Speed'
    
When I receive 'Speed'
* Hide

When I receive 'Game Over'
* Hide

When 'Flag' Clicked
* Hide
* Forever
  * Wait random time 15-25 seconds
  * Show
  * Go to a random position on the screen

## Meteor Shower
When 'Flag' Clicked
* Forever
  * If touching the ball
    * Then broadcast 'Game Over'
    
When I receive 'Game Over'
* Switch the background to 'Game Over'
* Hide

When 'Flag' Clicked
* hide
* Go to one of five designated locations for each meteors
* Start Meteor Shower

Define 'Meteor Shower'
* Forever
  * Wait 27 seconds
  * Switch the background to 'Meteor Shower'
  * Wait 3 seconds
  * Switch the background back to the white screen
  * Show
  * Glide 1 second to a random location at the bottom of the screen
  * Hide
  * Go back to original spot
