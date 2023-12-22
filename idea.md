Keep track of:  

ballPos(x,y)  
ballVel(x,y)  
playerA(y)  
playerB(y)  


Each cycle:  
  Update pos of players  
    Poll controllers  
    Determine if move allowed  
    Move  
  Update state of ball  
    Test for gameover  
      if ballPosX == minX || maxX
      GAMEOVER
    Test for wall contact  
      if ballPosY == minY || maxY
        Flip ballVelY
    Test for player contact  
      if ballPosX adjacent to player
        calc diff in ballPosX and playerX
          if in bounds
            update ballVelYaccording to diff and flip and increase ballVelX
 Move ball
   ballPosXY += ballVelXY
