# Blaze - A file sharing web app

Blaze is a file sharing web app that uses WebSockets and WebRTC to transfer files between multiple devices.
It currently uses `socket.io` to make real time connections on `express` backend. The frontend is built on vanilla JavaScript.
The current method of sharing files involves using base64 encoded format to transfer files. This may change to increase the efficiency of file transfer.


## Project structure
The project is divided into the backend and the frontend.


### Backend
Right now, only `index.js` file contains all the server-side code required for the backend. It is built on `express` and `socket.io` which allows usage of WebSockets and WebRTC. We may switch to using WebSockets natively as it is supported in almost all modern browsers.

### Frontend
All the frontend code is in the `public` folder. Once the frontend is built for production, all the built files are stored in `dist` folder which can be deployed along with the server code.

- No UI library is being used as of now.
- Sass is used for CSS pre-processing.


## Development
```bash
git clone https://github.com/blenderskool/blaze
cd blaze
npm install
npm run dev
```
The server by default would run on port `3030`

## Building for production
```bash
npm run build
```
The frontend built code would be located in the `dist` folder

## License
Blaze is [MIT Licensed](https://github.com/blenderskool/blaze/blob/master/LICENSE.md)