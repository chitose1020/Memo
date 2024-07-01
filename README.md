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
