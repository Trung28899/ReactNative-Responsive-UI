## 1. Core Knowledge:

    - Dimension API: Core API that allows code to get device width,
    height and more

    PACKAGES:
        $ expo install expo-app-loading
        $ npm install --save expo-font

    - In app.json:
        +, "orientation": "portrait"
        +, "orientation": "landscape"
        +, "orientation": "default"

## 2. Module Notes:

    *, 3r Commit: Adaptive Styling Rules and Dimensions API

        - Apaptive Styling
            +, ./screens/StartGameScreen.js:
            +, See inputContainer in styles object to see how
            to styles components by %

        - Dimension API:
            +, ./screens/StartGameScreen.js
            +, ./screens/GameScreen.js
            +, Search for 'Dimensions' and see how it is used

    *, 4th Commit: More example about Dimensions API

        - Should style properties based on Dimensions
        - The numerice values of the style properties are
             in pixels
        - ./screens/GameOverScreen.js: look for imageContainer
            styling to see how to work Dimensions

    *, 5th Commit: KeyboardAvoidingView API, Start working
        with Landscape screen

        - ./screens/StartGameScreen.js
        - Look for KeyboardAvoidingView
        - Suppose to push the screen to when input open keyboard
            But currently not affected
        > Need look into more if need to use

    *, 6th Commit: Listen to orientation change, create an event
        listener when the user rotate the device

        - ./screens/StartGameScreen.js
        - See code and comment in useEffect()
        - See how buttonWidth is used

## 3. Summary:

## 4. Useful Resources and Links:
