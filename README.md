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
