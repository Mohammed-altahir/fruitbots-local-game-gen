# fruitbots-local-game-gen
Python script to generate PvP Fruitbots games for local play.

# Please Note
This script expects Optimizely's fork of
[robot-fruit-hunt](https://github.com/optimizely/robot-fruit-hunt) to be in the
directory above this one because there is some file copying required to make
games work as expected.

Also note that this was built with a few assumptions in mind:
1. You cloned `robot-fruit-hunt` to the above directory without changing the
   name.
2. Your `open` command acts like OS X's.

# Usage
`game.py` is used to generate player vs player matches of fruitbots for local
play. It uses the `bots/` directory of `../robot-fruit-hunt` to generate games.

Let's say you wanted `dae-ho.js` to play against `nick.js`. To do that, you
would run:
```bash
python game.py dae-ho nick
```

The script will open the generated game's `game.html` in your browser where you
can manually begin the match.
