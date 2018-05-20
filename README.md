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
- manually edited the paths to .json files and into two .js files
- manually renamed images in dist/img folder to their original names
- and finally made a commit and pushed the project to github

