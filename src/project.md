Topic:-How to install new version of Tailwind css 4 in React project using vite

step 1:- create the  your project folder
   ---> mkdir project

 step 2:-open the project with vscode and open it terminal and write following command
   ---> npm create vite@latest

 step 3: write the project name as react_application (project name according to requirement)
  ----> project name :-----react_appication

step 4:- choose the framework
 ----> React

step 5:- choose the language
 ---> javascript

step 6:- follow this command
   -----> cd react_application
   -----> npm install
   ----->npm run dev

step 6: install the tailwind cee 4 in react. open terminal and follow this command
  --->  npm install tailwindcss @tailwindcss/vite

step 7: in the react_application folder stucure see the vite.config.js and add on few line 
     ---> import tailwindcss from '@tailwindcss/vite'
     ----> plugins: [
    tailwindcss(),
  ],

  after appling this line will be vite.config.js reflect like this

  import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import tailwindcss from '@tailwindcss/vite'

// https://vite.dev/config/
export default defineConfig({
  plugins: [react(),   tailwindcss(),],
})


step 7: go to the index.css and import this line on top
     ---> @import "tailwindcss";

step 8 :- run the project
    ---> npm run dev

step 9 add tailwind css classes like this 
      ---->   <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>    

step 10 :- run the project
    ---> npm run dev  