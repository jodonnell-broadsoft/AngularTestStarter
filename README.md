![alt tag](https://travis-ci.org/jonny2779/AngularTestStarter.svg?branch=master)
AngularTodo
===========

An app to test out basic AJS along with Jasmine, Karma and Travis

```
How to get testing working for JS and AJS

Install Jasmine by copying the files from here…

https://github.com/pivotal/jasmine/releases

lib is the folder that has the src of jasmine that you need.
spec has your tests in it.
src has your code in it.

Run the tests manually with SpecRunner.html.
(All files that you make and test need to be added to this file in order to be tested.)

Install Karma

npm install karma --save-dev
npm install karma-jasmine karma-chrome-launcher --save-dev

npm install -g karma-cli (ONCE Per dev only)

karma init
<enter>
<enter>
<enter> 
<enter> 
spec/*Spec.js
<enter> 
<enter> 

karma start (leave this open while you code in a terminal window)

karma run

Travis
Go to the Travis settings and enable travis for the repo. You will have to pay with Bill’s account

add .travis.yml to the repo with:

language: node_js
node_js:
  - 0.10
before_script:
  - export DISPLAY=:99.0
  - sh -e /etc/init.d/xvfb start

add a package.json file with:

{
    "name": "AngularTestStarter",
    "branchVersion": "1.0",
    "repository": {
        "type": "git",
        "url": "https://github.com/jonny2779/AngularTodo.git"
    },
    "devDependencies": {
        "karma": "~0.10"
    },
    "scripts": {
        "test": "karma start --single-run --browsers PhantomJS"
    }
}

Then add the build image to the readme (i.e. ![alt tag](https://travis-ci.org/jonny2779/AngularTestStarter.svg?branch=master))

```






