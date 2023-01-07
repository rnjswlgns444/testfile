# testfile
#testproject
import pygame
pygame.init()

WHIETE = (255,255,255)
size = (400, 300)
screen = pygame.display.set_mod(size)

done = False
clock = pygame.time.Clock()

airplane = gygame.image.load('images/plane.png')
airplane = pygame.transform.scale(airplane, (60,45))

def runGame():
  global done, airplane
  x=20
  y=24
  
  while not done:
    slock.tick(10)
    screen.fill(WHIETE)
    
    for event in pygame.event.get():
      if event.type == pygame.QUIT:
        done = True
      if event.type = pygame.KEYDOWN:
        if event.key == pygame.K_UP:
          y -= 10
        elif event.key == pygame.K_DOWN:
          y+= 10
  screen.blit(airplane, (x,y))
  pygame.display.update()
runGame()
pygame.quit()
