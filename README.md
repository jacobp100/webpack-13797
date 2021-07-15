# Webpack-13797

Run `yarn` and `yarn start`. Navigate to `localhost:3000`.

Please make sure you use `yarn` to get the same packages!

Steps

1. The main package imports two remotes.

2. Each remote sets a share scope - and the share scopes are the same.

3. When each remote loads, it logs its version of React.

4. The two remotes log the same version of React.

5. Check the network tab - two network requests for React are sent. There should only be one, as they are in the same share scope.
