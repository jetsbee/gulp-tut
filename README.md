# glup tutorial
- ref. https://github.com/nomadcoders/super-gulp
- ref. https://meyerweb.com/eric/tools/css/reset/

## Requirements (MacOS)
- A 64-bit Intel CPU 1
- macOS High Sierra (10.13) (or higher)

## Setup dev env (MacOS)
- Install Command Line Tools (CLT) for Xcode
```
$ xcode-select --install
```
- Install Homebrew
```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
- Install Nodejs
```
$ brew install node
```
- Install Yarn
```
$ brew install yarn
```

## Init node project
```
$ yarn init
```

## Add dependencies
```
$ yarn add gulp-cli gulp @babel/{core,register,preset-env} -D
```

## Make babelrc file
```
$ touch .babelrc
```
### .babelrc
```
{
  "presets": ["@babel/preset-env"]
}
```

## Make gulpfile
```
$ touch gulpfile.babel.js
```

## Add scripts to package.json
```
"scripts": {
    "dev": "gulp dev",
    "build": "gulp build",
    "deploy": "gulp deploy"
  }
```