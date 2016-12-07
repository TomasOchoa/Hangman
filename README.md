# Hangman Game

My implementation of a hangman game.

## ToDo List

- [ ] Figure out requirements

### UI/UX

#### New Game
- [ ] Implement difficulties
    - [ ] Figure out available difficulty levels
        - [ ] Easy - Gives a short length word
        - [ ] Medium - Gives a word of medium length
        - [ ] Hard - Gives a word of longer length
    - **NOTE**:
        - Should there be some implementation that takes into consideration
        the amount of vowels in a word? (The less vowels the more consonants which leaves for a much more difficult word)

#### Options
- [ ] Figure out what options to include.
    - [ ] Option to play with categories?
        - [ ] On
            - If turned on, player will be given a word from a certain
            category, and shown which one it is.
            - Until player sets it off, each new word will come from a
            category and display it to user.
        - [ ] Off
            - If turned off, player will be given a random word.
    - [ ] Option to allow player to change the number of strikes allowed
        - [ ] Default - 6 strikes
            - In this order:
                1. Head
                2. Torso
                3. Left Arm
                4. Right Arm
                5. Left Leg
                6. Right Leg
        - [ ] Lenient - 10 Strikes
            - In this order (starting from where default left off):
                7. Eyes
                8. Nose
                9. Ears
                10. Mouth
    - [ ] Option to allow player to play with hints
        - [ ] Off
            - Default option
        - [ ] On
            - Player has the option to see a hint once per game
            - **NOTE**:
                - Should the hint be a free letter given to the player or should it be something like 'contains 3 vowels'?
    - [ ] Figure out what animations to use and how to implement them.
        - [Paper.js](http://paperjs.org/)?
        - [Animate.css](https://daneden.github.io/animate.css/)?
        - [Bounce.js](http://bouncejs.com/)?
        - [Magic Animations CSS3](https://www.minimamente.com/example/magic_animations/)?
        - [DynCSS](http://www.vittoriozaccaria.net/dyn-css/#what-is-it)?
        - [CSShake](http://elrumordelaluz.github.io/csshake/#1)?
        - [Hover.css](http://ianlunn.github.io/Hover/)?
        - [Velocity.js](http://velocityjs.org/)?
        - [AniJS](http://anijs.github.io/)?

### Back-end/Functionality
- [ ] Figure out where to get words from
    - API?
        - Are there any APIs or libraries that get random words?
        - Checkout old TCP/IP project that connected to [dict server](http://www.dict.org/bin/Dict) that follows that RFC.
    - Database?
        - NoSQL?
            - Mongo?
            - FireBase?
        - SQL?
            - I only have experience using PostgreSQL
        - **NOTE**:
            - My hosting server uses SQL databases.
            - If I was to serve the game from my domain server, would I
            be able to create my own custom SQL Database for the game and
            use it this way?