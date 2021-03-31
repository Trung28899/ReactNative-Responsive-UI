## 1. Core Knowledge:

    - Dimension API: Core API that allows code to get device width,
    height and more

    PACKAGES:
        $ expo install expo-app-loading
        $ npm install --save expo-font
        $ expo install expo-screen-orientation

    - In app.json:
        +, "orientation": "portrait"
        +, "orientation": "landscape"
        +, "orientation": "default"

## 2. Module Notes:

    *, 11st Commit: Platform Specific Code Files
        - See the following files:
            +, ./components/MainButton.android.js
            +, ./components/MainButton.ios.js
            +, Import as MainButton in StartGameScreen.js
        - React Native will automatically choose the correct file
            for correct platform, no need to check platform

    *, 10th Commit: Working with Platform.select() and Platform
        in "if" Checks
        - Slick way to use Platform without using if check
            statement
        - ./components/Header.js
        - ./components/MainButton.js

    *, 9th Commit: Styling based on platform
    (IOS or Android)
        - Platform API is used to detect the platform
            user running on
        - See ./components/Header.js to see how this
            API is used

    *, 8th Commit: Introducing ScreenOrientation API
                (Only available in Expo)
        - Can lock a specific screen in 1 orientation
            try in GameScreen:
            ScreenOrientation.lockAsync(ScreenOrientation.OrientationLock.PORTRAIT);

        - Can listen and dectect orientation change:
            +, GameScreen.js
            +, Right now using get width from Dimensions
                Api to write adaptive code
            +, With ScreenOrientation can know for sure
                if the device is on Potrait or Landscape
                mode
            ScreenOrientation.addOrientationChangeListener();


    *, 7th Commit: Rendering Different layout on different dimensions

        - Use if statement with Dimensions API to check for
            Dimensions
        - See GameScreen.js for this

    *, 6th Commit: Listen to orientation change, create an event
        listener when the user rotate the device

        - ./screens/StartGameScreen.js
        - See code and comment in useEffect()
        - See how buttonWidth is used

    *, 5th Commit: KeyboardAvoidingView API, Start working
        with Landscape screen

        - ./screens/StartGameScreen.js
        - Look for KeyboardAvoidingView
        - Suppose to push the screen to when input open keyboard
            But currently not affected
        > Need look into more if need to use

    *, 4th Commit: More example about Dimensions API

        - Should style properties based on Dimensions
        - The numerice values of the style properties are
             in pixels
        - ./screens/GameOverScreen.js: look for imageContainer
            styling to see how to work Dimensions

    *, 3r Commit: Adaptive Styling Rules and Dimensions API

        - Apaptive Styling
            +, ./screens/StartGameScreen.js:
            +, See inputContainer in styles object to see how
            to styles components by %

        - Dimension API:
            +, ./screens/StartGameScreen.js
            +, ./screens/GameScreen.js
            +, Search for 'Dimensions' and see how it is used

## 3. Summary:

## 4. Useful Resources and Links:
