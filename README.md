# 2021 - 18 apr - notes

// (async () => { })()


# comments
pour lancer sans husky -->  git commit -n -m 'k'
angular - jasmin + karma pour tests

### yarn global
yarn global add firebase-tools      // npm install -g firebase-tools
yarn global add eslint
yarn global add sirv

### yarn
yarn init
yarn init
yarn -D firebase

### git
git init
git branch -M master
git remote add origin https://github.com/regnou/minimalist.git
git push -u origin master
// branch origin ?
git remote get-url --all origin

### firebase
firebase login
firebase use demofirebasesvelte
firebase init // firebase init hosting / firebase init functions

# starter
1 - firebase auth (just hosting is ok)
2 - firebase + firestore-manual-test
3 - 

### deploy
firebase deploy
firebase deploy --only hosting

### deploy combos (tu change de project a l interieur de la m app)
firebase use --add maconerie
firebase target:apply hosting maconerie app-maconerie
firebase target:clear hosting crm
firebase deploy --only hosting:axel-maconerie

### deploy static build sapper on firebase
alias task1='cd $HOME/0HOME/0GIT/GEN/ax-firebase-sapper/sapper && yarn export'
alias task2='cd $HOME/0HOME/0GIT/GEN/ax-firebase-sapper/firebase && firebase deploy --only hosting

# libs
## create own libs on NPM
npm login --registry=https://npm.pkg.github.com --scope=@regnou
pwd npm login --registry=https://npm.pkg.github.com --scope=@regnou
// github axel token = 253ac2d17c2534611bb25abfd4e54435ec8ff6c1

ya regnou/wc/wc-category 
//! UNIX ===================================================
find / -name abc.dmg

//! GIT ====================================================
// see large files
git ls-tree -r -t -l --full-name HEAD | sort -n -k 4

// pending push ?
git diff --stat --cached origin/master

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
