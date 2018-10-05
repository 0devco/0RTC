
# install

```bash
# npm
npm install @0devco/getusermedia
# yarn
yarn add @0devco/getusermedia
```

# use

```js
import getUserMedia from '@0devco/getusermedia'
getUserMedia({video: true, audio: false},function (err, stream) {
    // if the browser doesn't support user media
    // or the user says "no" the error gets passed
    // as the first argument.
    if (err) {
       console.log('failed');
    } else {
       console.log('got a stream', stream);  
    }
});

```
