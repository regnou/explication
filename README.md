# explication


# pre requisite
VS
ctrl P - shell command

# dependencies (nvm... already installed)
# yarn global
yarn global add firebase-tools      // npm install -g firebase-tools
yarn global add eslint
yarn global add sirv

# yarn
yarn init
yarn init
yarn -D firebase
 
# git
git init

# firebase
firebase login
firebase use demofirebasesvelte
firebase init



# starter
1 - firebase auth (just hosting is ok)
2 - firebase + firestore-manual-test
3 - 

# build
## DEV MODE

  # build firebaase
    - firebase start
    - firebase emulator

  - auto-reload : utiliser Open WC (prend 'node-resolve' et auto-reload)
   
## PROD MODE

# deploy
  firebase deploy
  firebase deploy --only hosting






# firebase CSR (no use of node, not included via bundler)


<script src="/__/firebase/8.2.10/firebase-app.js"></script>
<script src="/__/firebase/8.2.10/firebase-auth.js"></script>
<script src="/__/firebase/8.2.10/firebase-firestore.js"></script>
<script src="/__/firebase/init.js"></script>


npx create-snowpack-app dir-name --template svelte-tailwind-snowpack

