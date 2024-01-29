# react-xo-app
## Here I try to incorporate Tic-Tac-Toe app react code from React official tutorial into create-react-app template, to study basic of react template structure.

Here's the link to Tic-Tac-Toe tutorial.
https://react.dev/learn/tutorial-tic-tac-toe

Since I was new to React, I was trying to understand React from the mentioned tutorial on the official site of React, all was good until then I was wondering, "where are these codes should be placed in the actual React structured app?" Since it's not html, which you can run directly with a browser.

So I Google'd and then came across this W3school tutorial.
https://www.w3schools.com/react/react_getstarted.asp

Ok! Let's start with all the steps I went though.

```bash
mkdir xo
cd xo
```

Within my IDE terminal console (I used VScode for this project) I made directory as above, get to the directory then create React template directories and files with

```bash
npx create-react-app xoapp
```

Now, you should have structured directories and files with in "xo" directory. Something like this.

```
xo
|xoapp
| |-node_modules
| |-public
| |-src
|.gitignore
|package-lock.json
|package.json
```

Main files that were modified are

```
/xo/xoapp/src/App.js
```

```
/xo/xoapp/src/index.css
```

On App.js the main Tic-Tac-Toe code will be pasted, in fact you can just paste the whole code there.

![image](https://github.com/pjbmann/react-xo-app/assets/90997972/9f48c748-4728-4cb3-a53f-08cdbc2c4c01)

As you can see, after pasting code and saved, the page refresh to a familiar Tic-Tac-Toe game already!

![image](https://github.com/pjbmann/react-xo-app/assets/90997972/708cc977-6ea5-4cb8-83b1-e3740e4f3ca4)

## Now it's time for CSS styling.

On index.css file I added these so the page looks a bit more appealing and easier to see.

```css
.square {
  height: 100px;
  width: 100px;
  font-size: 50px; 
}
```

![image](https://github.com/pjbmann/react-xo-app/assets/90997972/12643dec-c9e0-4aa2-8081-e4d9557f2a27)

I know right, what happened!? Why are there these space when the button is pressed.
Don't worry I found the solution on good old StackOverFlow. xD
https://stackoverflow.com/questions/10575220/whats-with-the-space-above-button-element

```css
.square {
  height: 100px;
  width: 100px;
  font-size: 50px; 
  vertical-align: top; 
}
```

![image](https://github.com/pjbmann/react-xo-app/assets/90997972/fa567388-1f31-49b5-8673-df6e81158fa5)

YAY! I think this looks nice now.

Ok we are done here, so I came to conclusion that the main app should be coded in /src/App.js and you can just styling like normal CSS.

This is a good start for me to understand React :)

