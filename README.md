# What Should I Eat?

A small web app that helps pick dinner. You answer 11 quick questions (hunger, light or heavy, flavors, heat, hot or cold, texture, base, protein, familiar or new, cooking or ordering, and any hard no's), and it prints a pick on a diner-style order ticket.

## Running it

It's a single file with no build step. Open `index.html` in a browser.

It's also published as a Claude artifact: https://claude.ai/artifact/DibZxyR4Bvjve1wHw9s66f

## How it works

- `RAW` in `index.html` is the dish list (about 65 dishes). Each row has the dish's heaviness, portion size, flavors, spice level, temperature, textures, base, proteins, dairy and gluten flags, how adventurous it is, and how much effort it is to make at home.
- `score()` turns the answers into points per dish. Spice limits and dietary hard no's count much more than everything else, so you don't get something too hot or something you ruled out.
- "Not feeling it, 86 it" crosses off the current pick and shows the next best one.

## Ideas for later

- Add more dishes, or let people add their own
- Remember dishes that got 86'd often
- Two-person mode where both people answer and it finds the overlap
