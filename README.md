# Expo Image Component URI Formatting Issue

This repository demonstrates a bug in Expo's `Image` component where improperly formatted URIs can lead to unexpected behavior, such as the image failing to load or the application crashing.  The issue is exacerbated by the often-unclear error messages provided by Expo, making debugging challenging.  This repository provides example code showcasing the issue and a solution to mitigate the problem.

## Reproducing the Bug

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app using Expo Go or a similar tool.
4. Observe that the image in `bug.js` fails to load due to the extra space in the URI. 

## Solution

The solution involves carefully validating and cleaning the URIs before passing them to the `Image` component.  The `bugSolution.js` file demonstrates the use of a helper function to trim extra whitespace and ensure the URI is correctly formatted. 

## Contributing

Contributions are welcome! Feel free to submit pull requests to improve the code or documentation. 
