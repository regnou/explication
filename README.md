# explication

# comments
pour lancer sans husky -->  git commit -n -m 'k'
angular - jasmin + karma pour tests

# pre requisite
VS
ctrl P - shell command

# dependencies (nvm... already installed)
# yarn global
yarn global add firebase-tools      // npm install -g firebase-tools
yarn global add eslint
yarn global add sirv

### yarn
yarn init
yarn init
yarn -D firebase
 
### git
git init

# firebase
firebase login
firebase use demofirebasesvelte
firebase init // firebase init hosting / firebase init functions

# starter
1 - firebase auth (just hosting is ok)
2 - firebase + firestore-manual-test
3 - 

# build
## DEV MODE . . . . . . . . . . . . . . . . . . . . . 

  # build firebaase
    - firebase start
    - firebase emulator

  - auto-reload : utiliser Open WC (prend 'node-resolve' et auto-reload)

## PROD MODE . . . . . . . . . . . . . . . . . . . . . 

# deploy
  firebase deploy
  firebase deploy --only hosting

 # deploy combos (tu change de project a l interieur de la m app)
  firebase use --add maconerie
  firebase target:apply hosting maconerie app-maconerie
  firebase target:clear hosting crm
  firebase deploy --only hosting:axel-maconerie

# deploy static build sapper on firebase
  alias task1='cd $HOME/0HOME/0GIT/GEN/ax-firebase-sapper/sapper && yarn export'
  alias task2='cd $HOME/0HOME/0GIT/GEN/ax-firebase-sapper/firebase && firebase deploy --only hosting

# libs
 ## create own libs on NPM
  npm login --registry=https://npm.pkg.github.com --scope=@regnou
  pwd npm login --registry=https://npm.pkg.github.com --scope=@regnou
  // github axel token = 253ac2d17c2534611bb25abfd4e54435ec8ff6c1

# man
 ## sapper
  npm run dev — start the app in development mode, and watch source files for changes
  npm run build — build the app in production mode
  npm run export — bake out a static version, if applicable (see )
  npm start — start the app in production mode after you've built it

 ## firebase CSR (no use of node, not included via bundler)
  <script src="/__/firebase/8.2.10/firebase-app.js"></script>
  <script src="/__/firebase/8.2.10/firebase-auth.js"></script>
  <script src="/__/firebase/8.2.10/firebase-firestore.js"></script>
  <script src="/__/firebase/init.js"></script>


# END


npx create-snowpack-app dir-name --template svelte-tailwind-snowpack

---

ya regnou/wc/wc-category 



//! UNIX ===================================================
find / -name abc.dmg

//! GIT ====================================================
// see large files
git ls-tree -r -t -l --full-name HEAD | sort -n -k 4

// pending push ?
git diff --stat --cached origin/master

// branch origin ?
git remote get-url --all origin

echo "# 3-ms" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/regnou/3-ms.git
git push -u origin master





//! OPEN-WC ===============================================
// GENERATOR
npm init @open-wc
npm install @regnou/wc/wc-slideshow


// (async () => { })()

  "husky": {
    "hooks": {
      "pre-commit": "lint-staged"
    }
  },
  "lint-staged": {
    "*.js": [
      "eslint --fix",
      "prettier --write",
      "git add"
    ]
  }




