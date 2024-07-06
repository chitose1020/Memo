# 画像を配列として読み込む
```js
const imgs = ["a.png","b.png","c.png"]
let img = [];
for(let i = 0; i < 3; i++){
 img[i] = new Image();
 img[i] = imgs[i];
}
```
画像がすべて読み込まれたか確認する場合、上の`for`文のループ内に、
```js
img[i].onload = () => {
 実行したい処理
}
```
とする
# URLが有効かどうかを調べる
URLが有効かどうかを調べるときは、`new URL();`で有効でないURLを指定するとエラーが発生するのを利用して、`try {}catch{}`を使って調べる。
```js
try {
 new URL(調べたいURL);
 //URLが有効な場合の処理
}catch{
 //URLが無効な場合の処理
}
```
# JavaScriptを使ってリダイレクトする
```js
window.location.href = "リダイレクトしたいURL";
```
# オブジェクトがHTMLElementか判定する
```js
if (Obj instanceof HTMLElement) {
 //HTMLElementである
}else{
 //HTMLElementではない
}
```
