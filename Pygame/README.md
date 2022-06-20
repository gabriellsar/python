# Pygame 🎮
```python
import pygame as py
from sys import exit

py.init()

screen = py.display.set_mode((1020, 720))
py.display.set_caption('Pygame Screen')
clock = py.time.Clock()

font = py.font.Font('AwesomeFonte.ttf', 175)

while True:
    for event in py.event.get():
        if event.type == py.QUIT:
            py.quit()
            exit()

    screen.fill("Black")

    font_surf = font.render('PYGAME PROJECTS', True, "#00EE6E")
    font_rect = font_surf.get_rect(center=(510, 360))

    screen.blit(font_surf, font_rect)

    py.display.update()
    clock.tick(60)
```
