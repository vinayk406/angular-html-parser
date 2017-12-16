# angular-html-parser
HtmlParser extracted from Angular 


## build
1. tsc ./index.ts --outDir ./tmp --target "es2015" --module "es2015"
2. rollup ./tmp/index.js --o ./dist/ngCompiler.umd.js -f umd --name ngCompiler
3. uglifyjs ./dist/ngCompiler.umd.js -c  -o ./dist/ngCompiler.umd.min.js

## usage
1. include ngCompiler.umd.min.js

```ts
  let parser = new ngCompiler.HtmlParser();
  parser.parse('input');
```
