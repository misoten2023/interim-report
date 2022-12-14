---
theme: default
titleTemplate: 'Smart Classroom'
info: false
download: false
exportFilename: interim-report
highlighter: prism
lineNumbers: true
codeCopy: true
monaco: false
remoteAssets: false
selectable: false
record: false
colorSchema: auto
routerMode: history
aspectRatio: 16/9
canvasWidth: 980
favicon: /fav.png
plantUmlServer: https://www.plantuml.com/plantuml
css: windicss
fonts:
  sans: Klee One
  serif: Yuji Syuku
defaults:
  layout: default
drawings:
  persist: false
  enabled: true
  presenterOnly: true
  syncAll: true
layout: cover
---

# Smart Classroom
AIの力で新しい教室の未来を！ 

<style>
h1 {
  @apply font-bold
}
</style>

<!--
それではOH445の中間報告を始めます。  
私たちが今回提案するのは `Smart Classroom` です。
-->

---

# 企画概要
『<span class="text-red-400 font-bold">AI×教育</span>』AIの力で新しい教室の未来を！  

### 教育の課題点

~ 教員の不足とそれに伴う生徒個人の指導不足 ~

<img class="w-xs mx-auto" src="/classroom.webp">
<img class="absolute top-70 left-98 w-[30px]" src="/sensor.webp">
<img class="absolute top-63 left-138 w-[40px]" src="/camera.webp">
<img class="absolute top-90 left-150 w-[30px]" src="/microphone.webp">

<!-- 吹き出しとかもろもろ -->
<div class="absolute top-55 left-60">
  <div class="speech-bubble-1">
    <ul>
      <li>温度センサー</li>
      <li>湿度センサー</li>
      <li>明るさセンサー</li>
      <li>CO2濃度センサー</li>
    </ul>
    で生徒の状態を管理
  </div>
</div>

<div class="absolute top-60 left-110">
  <div class="speech-bubble-2">
    黒板の脱却
  </div>
</div>

<div class="absolute top-45 left-140">
  <div class="speech-bubble-3">
    カメラで生徒の理解度や<br>
    興味関心を記録
  </div>
</div>

<div class="absolute top-80 left-165">
  <div class="speech-bubble-4">
    マイクで生徒の発言、<br>
    授業への参加率を記録。<br>
    先生の授業内容を記録。
  </div>
</div>

<div class="absolute top-118 left-140">
  <div class="speech-bubble-5">
    机に個人IDカードをかざすと<br>
    出席と学習ログを同時に行える
  </div>
</div>

<div class="absolute top-110 left-40">
  <div class="speech-bubble-6">
    学習ログをオンラインで管理。<br>
    オンライン授業でも<br>
    変わらない授業を受けられる。
  </div>
</div>

<style>
h1 {
  @apply font-bold bg-cyan-600 bg-gradient-to-tr from-cyan-300 to-sky-900 bg-clip-text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
企画の概要ですが、  
"『AI×教育』AIの力で新しい教室の未来を！"  
という企画です。    
具体的には、新しい教室はIoTを用いて様々なデータを収集します。  
それらのデータをAIが解析し新しい教室の未来を想像します。  

この画像のように、  
カメラで生徒の理解度や興味関心を記録したり、  
マイクで生徒の発言から授業への参加率を計算したり、  
先生の授業内容を記録するなどです。

では実際にどのように未来を創造するかですが...
-->

---

# 企画概要

### こんな未来が！

<div class="grid grid-cols-2 grid-rows-2 gap-4">
  <div>
    <img src="/robot.webp" class="w-auto h-[150px] mx-auto mb-2">
    <div class="text-center">
      1人1人専用のAI<br>
      (友達であり先生)
    </div>
  </div>
  <div>
    <img src="/door.webp" class="w-auto h-[150px] mx-auto mb-2">
    <div class="text-center">
      映像や学習ログから<br>
      出席や進捗を自動集計
    </div>
  </div>
  <div>
    <img src="/report.webp" class="w-auto h-[150px] mx-auto mb-2">
    <div class="text-center">
      AIが生徒の理解度や興味、関心を記録
    </div>
  </div>
  <div>
    <img src="/browser.webp" class="w-auto h-[150px] mx-auto mb-2">
    <div class="text-center">
      黒板からの脱却<br>
      誰もがどこからでも受けられる授業
    </div>
  </div>
</div>


<style>
h1 {
  @apply font-bold bg-cyan-600 bg-gradient-to-tr from-cyan-300 to-sky-900 bg-clip-text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
このような形です。

１人１人専用のAIがあり、先生として、友達として接することができたり、
先ほどの収集した映像や学習ログから、出席や進捗を自動集計、  
AIが生徒の理解度や興味、関心を記録、  
黒板から脱却することで、誰もがどこからでも受けられる授業  

などなど、の未来が想像できます。

これらの未来を実現するために私たちが作る機能のですが、いくつか紹介します...
-->

---

# 主要機能

## 授業内容のテキスト化

<br>

### 現状の問題点

- 授業を聞き逃してしまった
- 声が届かず聞こえなかった
- 耳が不自由で授業に参加できない
- 留学で日本語がまだ得意ではない

など、様々な場合で音声のみだと不便が生じることがあり、  
学業を困難にしてしまうことがあります。

<img src="/tablet.webp" class="absolute w-[300px] top-20 right-20">

<style>
h1 {
  @apply font-bold bg-cyan-600 bg-gradient-to-tr from-cyan-300 to-sky-900 bg-clip-text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
ではここからは先ほどの未来を想像するために今回実際に私たちが作成する機能例です。

機能例1です。  
授業内容のテキスト化です。  
マイクで収集した音声をテキスト化するものです。

//スライドを読む

これらを解決するために、マイクから収集した音声を自動で文字に起こしていきます。
また、留学生に対して、自動翻訳し苦手な言語でも学習しやすい環境を提供します。
-->

---

# 主要機能

## 集中力の可視化

<br>

### 現状の問題点

- 授業中は誰が集中しているかわからない
- 生徒は自分がどういう時に集中できるかわからない

といった集中しているかどうかが、定量的にわからず  
より良い成果の出し方が本人もわからない、  
授業中も全員を均等に見れないという現状があります。

<img src="/student.webp" class="absolute w-[300px] top-20 right-20">

<style>
h1 {
  @apply font-bold bg-cyan-600 bg-gradient-to-tr from-cyan-300 to-sky-900 bg-clip-text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!-- 
機能例3です。  
生徒の集中力をカメラから得た映像を用いて分析します。  
先生はどの生徒が授業に集中できているのか、リアルタイムで手元で確認できます。  
生徒も自分のどういったときに集中できているのか認識との乖離を確認できます。  
 -->

---
layout: center
---

## それでは実際に授業をやってみましょう！！