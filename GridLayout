import pygame
import sys

pygame.init()
screen = pygame.display.set_mode((300, 300))

grid = []
for rowthing in range(10):
    grid.append([])
    for column in range(10):
        grid[rowthing].append([])

for i in range(10):
    for u in range(10):
        pygame.draw.rect(screen, (255, 255, 255), (1 + i * 30, 1 + u * 30, 28, 28))


def main():
    while True:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                pygame.quit
                sys.exit()
            pygame.display.update()
            if event.type == pygame.MOUSEBUTTONDOWN:
                pos = pygame.mouse.get_pos()
                col = pos[1] // 30
                rowb = pos[0] // 30
                if rowb < 11 and col <11:
                    onclick(rowb, col)


def onclick(rowb, col):
    pygame.draw.rect(screen, (55, 55, 55), (1 + rowb*30, 1 + col*30, 28, 28))
    grid[rowb][col] = 1
    print("{0}{1}".format(str(rowb), str(col)))


main()
