# angular-test1

## installation

```
# wget https://nodejs.org/dist/v12.18.3/node-v12.18.3-linux-x64.tar.xz
# mkdir -p /usr/local/lib/nodejs
# tar -xJvf node-v12.18.3-linux-x64.tar.xz -C /usr/local/lib/nodejs

# vim .bashrc
```
```
export PATH=/usr/local/lib/nodejs/node-v12.18.3-linux-x64/bin:$PATH
```
```
# node --version
v12.18.3
```
```
# npm install -g @angular/cli
```
```
# ng --version

     _                      _                 ____ _     ___
    / \   _ __   __ _ _   _| | __ _ _ __     / ___| |   |_ _|
   / △ \ | '_ \ / _` | | | | |/ _` | '__|   | |   | |    | |
  / ___ \| | | | (_| | |_| | | (_| | |      | |___| |___ | |
 /_/   \_\_| |_|\__, |\__,_|_|\__,_|_|       \____|_____|___|
                |___/


Angular CLI: 10.0.8
Node: 12.18.3
OS: linux x64

Angular:
...
Ivy Workspace:

Package                      Version
------------------------------------------------------
@angular-devkit/architect    0.1000.8
@angular-devkit/core         10.0.8
@angular-devkit/schematics   10.0.8
@schematics/angular          10.0.8
@schematics/update           0.1000.8
rxjs                         6.5.5
```

## create project

```
# ng new angular-app
? Would you like to add Angular routing? No
? Which stylesheet format would you like to use? CSS
CREATE angular-app/README.md (1028 bytes)
CREATE angular-app/.editorconfig (274 bytes)
CREATE angular-app/.gitignore (631 bytes)
CREATE angular-app/angular.json (3606 bytes)
CREATE angular-app/package.json (1263 bytes)
CREATE angular-app/tsconfig.base.json (458 bytes)
CREATE angular-app/tsconfig.json (426 bytes)
CREATE angular-app/tslint.json (3184 bytes)
CREATE angular-app/.browserslistrc (853 bytes)
CREATE angular-app/karma.conf.js (1023 bytes)
CREATE angular-app/tsconfig.app.json (292 bytes)
CREATE angular-app/tsconfig.spec.json (338 bytes)
CREATE angular-app/src/favicon.ico (948 bytes)
CREATE angular-app/src/index.html (296 bytes)
CREATE angular-app/src/main.ts (372 bytes)
CREATE angular-app/src/polyfills.ts (2835 bytes)
CREATE angular-app/src/styles.css (80 bytes)
CREATE angular-app/src/test.ts (753 bytes)
CREATE angular-app/src/assets/.gitkeep (0 bytes)
CREATE angular-app/src/environments/environment.prod.ts (51 bytes)
CREATE angular-app/src/environments/environment.ts (662 bytes)
CREATE angular-app/src/app/app.module.ts (314 bytes)
CREATE angular-app/src/app/app.component.css (0 bytes)
CREATE angular-app/src/app/app.component.html (25725 bytes)
CREATE angular-app/src/app/app.component.spec.ts (957 bytes)
CREATE angular-app/src/app/app.component.ts (215 bytes)
CREATE angular-app/e2e/protractor.conf.js (869 bytes)
CREATE angular-app/e2e/tsconfig.json (299 bytes)
CREATE angular-app/e2e/src/app.e2e-spec.ts (644 bytes)
CREATE angular-app/e2e/src/app.po.ts (301 bytes)
✔ Packages installed successfully.
    Directory is already under version control. Skipping initialization of git.
```

- gitignore file is automatically configured.

```
# head -15 angular-app/.gitignore
# See http://help.github.com/ignore-files/ for more about ignoring files.

# compiled output
/dist
/tmp
/out-tsc
# Only exists if Bazel was run
/bazel-out

# dependencies
/node_modules

# profiling files
chrome-profiler-events*.json
speed-measure-plugin*.json
```

## start project

- "--host 0.0.0.0" option allows access outside localhost

```
# cd angular-app
# ng serve --host 0.0.0.0
```
```
WARNING: This is a simple server for use in testing or debugging Angular applications
locally. It hasn't been reviewed for security issues.

Binding this server to an open connection can result in compromising your application or
computer. Using a different host than the one passed to the "--host" flag might result in
websocket connection issues. You might need to use "--disableHostCheck" if that's the
case.

(snip)

** Angular Live Development Server is listening on localhost:4200, open your browser on http://localhost:4200/ **
: Compiled successfully.
```

## access project page

```
http://<ip address>:4200/
```

![alt text](https://hirofumi-github-images.s3.amazonaws.com/angular-test-top.JPG)

