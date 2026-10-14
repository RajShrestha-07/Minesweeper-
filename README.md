# Minesweeper

Minesweeper is a small web game. A 9x9 board hides 10 mines. Open the safe squares, and each number tells you how many mines touch that square. Flag the squares you think are mines. Your first tap is always safe, there is a timer, and you can switch between Dig and Flag mode, so it works on a phone without a right click.

Live demo:

Built with: HTML, CSS and JavaScript.

What this project shows: The mines are not placed until your first tap, and they avoid that square and its neighbours, so you can never lose on the first move. Each square's number is found by counting the mines in its up to 8 neighbours. When you open a square with a zero, the game opens its neighbours automatically, and keeps going outward. It does this with a stack instead of repeating the same code, which is a flood fill, the same idea as the paint bucket tool in an image editor. The board is stored in simple lists of true and false values, one for mines, one for opened squares and one for flags.

What I'm learning from it: I'm studying how the `neighbors` function finds the squares around a square, how `place` avoids the first tap, and how `reveal` uses a stack to open many squares at once.
