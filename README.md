# Belajar-tailwind-Css-wpu
[Documentasi Tailwind Css](https://tailwindcss.com/docs/installation)

- Pertama yang harus kita lakukan npm init terlebih dahulu.
`npm init`
- Install Tailwind Css, postcss, autoprefixer.
`npm install -D tailwindcss postcss autoprefixer`
- buat file **tailwind.config.js** dengan cara ketik di terminal `npx tailwindcss init`
- maka akan di buatkan template.
```js module.exports = {
  content: ["./public/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
- buat sebuah folder **_src/css/input_** dan masukan script 
```js
@tailwind base;
@tailwind components;
@tailwind utilities;
```
- jalan kan sebuah proses buildnya dengan mengetikan di terminal.
`npx tailwindcss -i ./src/css/input.css -o ./public/style.css --watch`
- proses setup tailwind css terakhir adalah dengan memasukan code di `index.html` 
```js
 <link href="/public/css/style.css" rel="stylesheet">
 ```
