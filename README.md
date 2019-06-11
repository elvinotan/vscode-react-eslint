# Visual Studio Code / React Programing/ Eslint Setup

# DOWNLOAD AND INSTALL VSCODE 
Download from https://code.visualstudio.com/</br>

Linux :</br>
sudo dpkg -i {deb filename} </br>


# CREATE NEW REACT NATIVE APP 

react-native init {project name}</br>


# INSTALL ESLINT 3:26

(1) Install eslint plugins</br>

npm install --save-dev babel-eslint eslint eslint-config-google eslint-plugin-babel eslint-plugin-jest eslint-plugin-react</br>
atau</br>
Add this code into package.json </br>
```
"babel-eslint": "^8.2.1",
"eslint": "^4.15.0",
"eslint-config-google": "^0.9.1",
"eslint-plugin-babel": "^4.1.2",
"eslint-plugin-react": "^7.5.1",
"eslint-plugin-react-native": "^3.2.1",
```
```
lalu jalankan npm install
```

(2) Install esLint vscode plugin

(3) Create .eslintrc file in the project and add the following code,
```
{
  "extends": ["eslint:recommended", "plugin:react-native/all", "plugin:react/all", "google", ],
  "globals": {
    "require": false,
  },
  "plugins": [
    "react",
    "babel",
    "react-native"
  ],
  "env": {
    "es6": true,
    "node": true,
    "browser": true
  },
  "ecmaFeatures": {
    "jsx": true,
    "modules": true
  },
  "parser": "babel-eslint",
  "parserOptions": {
    "sourceType": "module",
    "ecmaFeatures": {
      "jsx": true
    }
  },
  "rules": {
    "indent": ["error", 2],
    "new-cap": 0,
    "max-len": [2, 120],
    "no-undef": 2,
    "require-jsdoc": 0,
    "react/forbid-component-props": 0,
    "react/forbid-prop-types": 0,
    "react/jsx-indent": [2, 2],
    "react/jsx-indent-props": "off",
    "react/jsx-no-literals": 0,
    "react/jsx-filename-extension": 0,
    "react/no-set-state": 0,
    "react/prefer-stateless-function": [2, { "ignorePureComponents": true }],
    "react/no-multi-comp": [2, { "ignoreStateless": true }],
    "react/jsx-one-expression-per-line": 0,
    "react/destructuring-assignment": 0,
    "no-invalid-this": 0,
    "babel/no-invalid-this": 2,
    "react/no-access-state-in-setstate": 0
  }
}
```

# INSTALL FLOW

(1)Find the Flow [version] at the bottom of the included .flowconfig</br>
(2) npm install --save-dev flow-bin@x.y.z </br>
(x.y.z is the .flowconfig version number)</br>
(3)Install VS code flow plugin
