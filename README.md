# 4.2.2import pygame
import sys
pygame.init()
screen_width = 800
screen_height = 800
title = "Пример"
background_color = (68, 255, 0)
screen = pygame.display.set_mode((screen_width, screen_height))
pygame.display.set_caption(title)
while True:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()
    screen.fill(background_color)
    pygame.display.flip()
