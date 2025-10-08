---
layout: ../layouts/ProjectLayout.astro
title: "WordleCrack - 破解Wordle"
publishDate: "2024-10-26"
tags: ["Python", "CLI Tool", "Algorithm", "Wordle"]
description: "一個命令列工具，透過字母頻率分析與刪去法，為熱門猜字遊戲 Wordle 提供最佳猜測建議。"
---
<!-- ABOUT THE PROJECT -->
## About The Project

WordleCrack is a command-line interface (CLI) tool designed to help players solve the daily Wordle puzzle more efficiently.

When a player inputs the hints from the game (green, orange, and gray letters), the tool calculates and recommends the most effective next guess based on its built-in word list and English letter frequency data, speeding up the solving process.

### Core Features

* **Smart Recommendations**: On the first turn, it suggests words that are most likely to contain multiple common letters.
* **Precise Filtering**: Quickly narrows down the pool of possible words based on user input for `g` (green), `o` (orange), and `-` (gray) hints.
* **Interactive Interface**: Allows users to play through multiple rounds of guesses in the terminal until the answer is found.
* **Dynamic Strategy**: In the early stages of the game, the algorithm prioritizes suggesting words that explore more "unknown" letters to maximize information gain.

### Built With

[Python](https://www.python.org/)

<!-- GETTING STARTED -->
## Getting Started

Follow these steps to get a local copy up and running.

### Prerequisites

* **Python 3.x**: Ensure you have Python 3 or a later version installed on your system.

### Installation and Execution

1. Clone this repo

    ```sh
    git clone https://github.com/0oWoodenDooro0/WordleCrack.git
    ```

2. Navigate to the project directory

    ```sh
    cd WordleCrack
    ```

3. Run the main script

    ```sh
    python main.py
    ```

<!-- USAGE EXAMPLES -->
## Usage

The program starts by recommending 5 initial words.

```
salet
crate
trace
slate
crane
```

Next, follow the prompts to enter your guess and the color feedback provided by Wordle.

**Color Codes:**

* `g` = green (letter is in the correct position)
* `o` = orange (letter is in the word but in the wrong position)
* `-` = gray (letter is not in the word)

```
Enter word: raise
Enter color: -o-g-
```

The program will then calculate and display the best words for the next guess based on your feedback. Repeat this process until you find the answer. You can type `end` to start a new game.

<!-- CONTACT -->
## Contact

[Vincent] - [vincent031525@gmail.com]

Project Link: [https://github.com/0oWoodenDooro0/WordleCrack](https://github.com/0oWoodenDooro0/WordleCrack)
