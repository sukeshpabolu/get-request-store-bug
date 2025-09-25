## To reproduce the bug
- clone the repo
- install the packages using `npm install`
- go to `$lib/bundle.js`
- Comment this line
  `export const bundlePath = assets("/example.js");`
- Uncomment this line
  `export const bundlePath = `${assets}/example.js`;`
- Run `npm run dev` 
- You will encounter `get_request_store` error.
