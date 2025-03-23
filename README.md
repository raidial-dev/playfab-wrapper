# PlayFab API Wrapper

A very simple and easy to use API wrapper which uses the PlayFab API to do many features such as banning users, granting items, and much more.

## Installation
To install the package, run:
```sh
npm install playfab-wrapper
```
## Example
Note: The duration in the example below is in hours.

```js
const PlayFabAPI = require("playfab-wrapper");
const playfab = new PlayFabAPI("TitleID", "SecretKey");

async function BanPlayer() {
    const result = await playfab.BanUser("UserID", "Reason", 24);
    console.log(result);
}

BanPlayer();
```
