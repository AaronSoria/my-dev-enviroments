#A dev enviroment with node, vue and tailwindcss

Now, let’s create a new vue.js app using vue create <app-name>
  
$ vue create <app-name>

Now, let's install the dependencies required to work with Tailwind.
  
$ npm install tailwindcss@npm:@tailwindcss/postcss7-compat postcss@^7 autoprefixer@^9

After run docker image you should run 

npx tailwindcss init -p

Open your app in your favorite editor.
In the tailwind.config.js file,
- replace purge: []
- with purge: [‘./index.html’, ‘./src/**/*.vue,js,ts,jsx,tsx}’]

Under the src folder create index.css and add the following.
/* ./src/index.css */
@tailwind base;
@tailwind components;
@tailwind utilities;


In the main.js file, import index.css

|       import Vue from 'vue'               |
  
|       import App from './App.vue'         |
  
|       import router from './router'       |
  
|       import store from './store'         |
  
|       import './index.css'                |

reference
https://medium.com/featurepreneur/set-up-tailwind-css-for-your-vue-js-app-5a8801fd0a55
