# processing程式設計與 p5.js設計
processing程式設計
* [官方網站](https://p5js.org/)([中文網站](https://p5js.org/zh-Hans/))
* [線上編輯](https://editor.p5js.org/p5/)
* 需要的基本檔案


[學習網站內容整理](https://p5js.org/zh-Hans/learn/)
[指令查詢](https://p5js.org/zh-Hans/reference/)

# 基本兩個函數(function)

## 產生一個背景顏色
### 背景指令:[background(220)](https://p5js.org/zh-Hans/reference/#/p5/background)
---


劃出一個圓
[畫橢圓(圓)指令](https://p5js.org/zh-Hans/reference/#/p5/ellipse)
```
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
  ellipse(50,50,80,80); //圓心為(50,50)，寬為80，高為80，所以是個圓
}
```
![](https://i.imgur.com/xgxur8S.png)


---


當滑鼠按鈕一按後，產生黑色充滿的圓型
```
function setup() {
  createCanvas(400, 400);
}

function draw() {
  if (mouseIsPressed) {
    fill(0);
  } else {
    fill(255);
  }
  ellipse(mouseX, mouseY, 80, 80);
}
```

![](https://i.imgur.com/1LHQbvM.png)


---




另外的範例
* [p5.play]( p5play.molleindustria.org)
  * 範例下載
```
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
}
```
![](https://i.imgur.com/XHY4nvG.png)

