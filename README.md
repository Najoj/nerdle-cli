Work in progress

# wordle-cli

Command-line clone of klipspringr's [nerdle-cli](https://github.com/klipspringr/wordle-cli/) adapted for [Nerlde](https://nerdlegame.com/).

Customize solution, of customizable length.

## Download and run

Requires **Python 3.6** or later, and a **modern terminal app**.

To download the code and run it:

```bash
git clone https://github.com/klipspringr/wordle-cli.git && cd wordle-cli
python3 play.py
```

Alternatively, if you don't have git: click `Code > Download ZIP` on GitHub, extract the ZIP, open a terminal, `cd` to the extracted folder and run `python3 play.py`.

A **terminal with support for colours and emoji** is required. On Windows and WSL, [Windows Terminal](https://aka.ms/terminal) is the best choice. PowerShell and the Windows command prompt are only supported if running in Windows Terminal.

## Options

Usage: `python3 play.py [-h|--help] [--today|DAY|SOLUTION] [--hints]`

|Option                     |Behaviour                                                  |
|---------------------------|-----------------------------------------------------------|
|_none_                     |Use a random solution from the official Wordle dictionary  |
|`--today`                  |**\***  Use today's official Wordle solution               |
|`DAY` (number)             |**\***  Use the official solution from this DAY            |
|`SOLUTION` (string)        |**\***  Use a given SOLUTION (must be 5-letter word)       |
|`--hints`                  |After each guess, report number of possible words remaining|
|`-h` , `--help`            |Print this help text and quit                              |

_Note: options marked **\*** are mutually-exclusive._

So, to play against random solutions, run `python3 play.py`; to play today's official solution, run `python3 play.py --today`; or to play against the solution from game day 211 (16 January 2022), run `python3 play 211`. 

Hints mode (`--hints`) looks like this:

