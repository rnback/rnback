# rnback

Rnback is a __backend service__ for react-native applications.

To learn more, head to [https://rnback.com](https://rnback.com)


-----------------------

# rnback sdk

## Install

1. Create a react-native project: (If you don't already have one)
```bash
    react-native init MyProject && cd MyProject
```

2. Install the sdk:
```bash
    npm install --save rnback
```

3. Add key from the dashboard https://dashboard.rnback.com/ :
```bash
    node ./node_modules/rnback/cli/ setkey "<key from dashboard>"
```
 * NOTE: It's important to do this step before the following.

4. Link library
```bash
    react-native link rnback
```

5. Done! you can now use the sdk from your app
```javascript
    import {authenticate} from 'rnback';
    
    authenticate()
        .then(() => console.log('yay!'))
	    .catch(() => console.log('boo'));
```

---

