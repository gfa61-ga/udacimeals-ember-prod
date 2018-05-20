# UdaciMeals
[Live page](https://gfa61-ga.github.io/udacimeals-ember-prod/#/menu/) (links to item Details do NOT work..???)

To make this live version:

- in my PC I went to the udacimeals-ember folder,
- in config/environment.js file I added:

```
  if (environment === 'production') {
    // here you can enable a production-specific feature
    ENV.rootURL = '/udacimeals-ember-prod/';
    ENV.locationType = 'hash';
  }
  ```

- run:
```    ember build -prod```
- and then coppied the dist folder into the new udacimeals-ember-prod folder,
- manually edited the paths to .json files and into two .js files:
```
assets/udaci-meals-572f420663cbfd1421f7d1a46cc55b65.js
assets/udaci-meals-ffe32956b505d2b4ad503eecdfd5a9b4.js
```
- manually renamed images in dist/img folder to their original names
- and finally made a commit and pushed the project to github

[maybe this link can solve the Links issue](https://stackoverflow.com/questions/24404080/how-do-i-deploy-ember-js-app-developed-with-ember-cli-on-github-pages)
