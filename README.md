# hubot-trivia

A trivia script for Hubot.

    !trivia # start game
    !trivia help # see commands
    !hint # show hint
    !end # manual game end (debug only)
    
### Installation

1. Edit `package.json` and add `hubot-trivia` to the `dependencies` section. Example:


    ```javascript    
    "dependencies": {
      "hubot-trivia": ">= 0.3.0",
      ...
    }
    ```   
        

2. Add "hubot-trivia" to your `external-scripts.json`. Example:

    ```javascript
    ["hubot-trivia"]
    ```

3. Supply a question database and assign it to @dbfile. This version expects the following table structure:

    `table: questions`
    `fields: category text, title text`
    
    `table: answers`
    `fields: id integer, answer text`
    
    Each row in `questions` has a unique `rowid`. The `answers` table contains one or more accepted answers to each question, with `id` matching the question's `rowid`.
