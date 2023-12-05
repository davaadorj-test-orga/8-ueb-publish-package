# npm package
- edit package.json
````
npm init
````

important: name & repository
````
...
"name": "@davaadorj-test-orga/my-hello-world",
"repository": "https://github.com/davaadorj-test-orga/8-ueb-publish-package.git",
...
````

## publish from local
- add .npmrc to gitignore
- generate token - scope repo, workflow?, write&delete package
- add repo-url & token to the .npmrc file

````
npm.pkg.github.com/:_authToken=xxx
@davaadorj-test-orga:registry=http://npm.pkg.github.com
````

[see more details here](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-npm-registry)

````
cd sample-packages/npm
npm publish

or 

npm login --scope=@NAMESPACE --auth-type=legacy --registry=https://npm.pkg.github.com

> Username: USERNAME
> Password: TOKEN

````
# 