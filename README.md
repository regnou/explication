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

# yarn
yarn init
yarn init
yarn -D firebase
 
# git
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

---

ya regnou/wc/wc-category 

pwd npm login --registry=https://npm.pkg.github.com --scope=@regnou
github axel token = 253ac2d17c2534611bb25abfd4e54435ec8ff6c1
npm login --registry=https://npm.pkg.github.com --scope=@regnou
pwd npm login --registry=https://npm.pkg.github.com --scope=@regnou



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


//! FIREBASE ===============================================
 firebase use --add maconerie
firebase target:apply hosting maconerie app-maconerie
firebase target:clear hosting crm
firebase deploy --only hosting:axel-maconerie

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



