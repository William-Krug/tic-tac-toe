# App Set up Template (React w/Redux)

## Initial Installs

- [x] Run `npm init` from the terminal
- [x] Run `npm install express` from the terminal
- [ ] Run `npm install pg` from the terminal
- [x] Run `npm install axios` from the terminal
- [x] Run `npm install react` from the terminal
- [x] Run `npm install react-router-dom` from the terminal
- [ ] Run `npm install redux react-redux` from the terminal
- [ ] Run `npm install redux-logger` from the terminal
- [x] Run `npm install dotenv` from the terminal
- [ ] Run `npm install redux-saga` from the terminal

### `.env`

- [x] create `.env` file inside of the root directory
  - [x] add any key: value pairs to the file that need to be held private and not pushed to GitHub
  - [ ] add `require('dotenv').config()` to any files that require use of the secret keys

### `.gitignore`

- [x] Make sure the `.gitignore` file has:
  - [x] `node_modules/`
  - [x] `.DS_Store`
  - [x] `.eslintcache`
  - [x] `.env`

### `package.json`

- [x] Make sure the `package.json` file has:
  - [x] `"proxy": "http://localhost:5000"`
  - [x] `"client": "react-scripts start"` under the `"scripts"` section
  - [x] `"server": "nodemon --watch server server/server.js"` under the `"scripts"` section

## Server Side Setup

- [ ] Create `server` directory (if it doesn't already exist)
- [ ] Create `server.js` inside of the `server` directory
  - [ ] `const express = require('express')`
  - [ ] `const app = express()`
  - [ ] `const PORT = process.env.PORT || 5000`
  - [ ] `app.use(express.static('build'))`
  - [ ] `app.use(express.json())`
  - [ ] `app.use(express.urlencoded({extended: true})`
  - [ ] `app.listen(PORT, () => {console.log("Listening on port ${PORT}...."); })`

### Modules

- [ ] Create `modules` directory inside of the `server` directory (if it doesn't already exist)
- [ ] Create `pool.js` inside of the `modules` director
  - [ ] `const pg = require('pg')`
  - [ ] `const Pool = pg.Pool`
  - [ ] `const config = { database: 'databaseName', host: 'localhost' port: 5432, };`
  - [ ] `const pool = new pg.Pool(config);`
  - [ ] `pool.on("connect", (client) => {console.log('connected to postgres');});`
  - [ ] `pool.on("error", (error, client) => {console.log('Error: Connecting to postgres', error); process.exit(-1);});`
  - [ ] `module.exports = pool;`
- [ ] `const pool = require('filepath to pool.js')` where needed (most likely `server.js`)

### Routers

- [ ] Create `routes` directory inside of the `server` directory (if it doesn't already exist)
- [ ] add `.router.js` files as necessary to handle database requests

## Client Side Setup

### `App.js`

- [ ] Navigate to `/App.jsx` and add:
  - [ ] `import { HashRouter as Router, Route, Link, useHistory, } from 'react-router-dom'`
  - [ ] `import { useEffect } from 'react'`;
  - [ ] Add `<Router><Route path=''><Route></Router>` as necessary

### Axios

- [ ] `import axios from 'axios'` in any file making AXIOS calls
  - [ ] may need to use `import { axios } from 'axios'`

### Components

- [ ] Create a `components` directory inside of the `src` directory (if it doesn't already exist)
- [ ] inside of each component, add the following as necessary:
  - [ ] `import { useSelector, useDispatch } from 'react-redux'`
  - [ ] `const dispatch = useDispatch()`
  - [ ] `const variableName = useSelector((store) => {return store.whatYouWantFromTheStore;})` for each variable needed
  - [ ] `dispatch({type: 'MESSAGE_TO_SEND', payload: 'data_to_send'})` inside each handler

### Redux

- [ ] navigate to `/src/index.js` and add:
  - [ ] `import { createStore, combineReducers, applyMiddleware } from 'redux'`
  - [ ] `import { Provider } from 'react-redux'`
  - [ ] `import logger from 'redux-logger'`
  - [ ] `const reducerName = (state = 0, action) => {return state;}` for each reducer (variable) needed -> listed before next line
  - [ ] `const store = createStore(combineReducers({reducer1, reducer2, ...}),applyMiddleware(logger));`
  - [ ] `ReactDOM.render(<React.StrictMode><Provider store={store}><App /></Provider></React.StrictMode>,document.getElementByID('root'));`
- [ ] Navigate to and add to any file that needs data from the `store`

### Saga

- [ ] in `index.js`:
  - [ ] `import createSagaMiddleware from 'redux-saga`
  - [ ] `import { takeEvery, put } from 'redux-saga/effects'`
  - [ ] `function* watcherSaga() {yield takeEvery('dispatchAction', callSecondFunction);}`
  - [ ] `function* callSecondFunction() {try{let response = yield axios. ...yield put({type: '', payload: ...})} catch(error){...}}`
  - [ ] `const sagaMiddleware = createSagaMiddleware()`
  - [ ] add `sagaMiddleware` to the `store` in the `applyMiddleware()` section
  - [ ] `sagaMiddleware.run(watcherSaga)`
