Heroku 快速建立鬼扯LineBot-使用Python
===

現在聊天機器人非常火紅，今天帶大家來建立一個簡單的聊天機器人，機器人回的話是Call 我自己訓練的一些對話，因為沒有訓練得很好，所以他常常在鬼扯ＸＤ。下面不用寫<a href="https://github.com/NickYuu/Python_Line_Bot" style="color:blue;">程式</a>(我已經寫好了直接部署就能玩摟)

<br>

<a href="https://heroku.com/deploy?template=https://github.com/NickYuu/Python_Line_Bot">
<img src="https://www.herokucdn.com/deploy/button.svg" alt="Deploy"></img></a>


<br/>

點擊上方按鈕開始部署

<br>

<img src="https://i.imgur.com/gOSxJFo.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br/>

點擊Deploy

<br/>

<img src="https://i.imgur.com/uEJIakI.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br/>

跑完你的bot，已經部署上去摟！

---

接著我們需要開一個line bot帳號。
<a href="https://business.line.me/zh-hant/services/bot" style="color:blue;">Messaging API</a>


<br>

<img src="https://i.imgur.com/IIDKuVN.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

一路順著步驟最後會到 `Line@MANGER` 頁面

<br>

<img src="https://i.imgur.com/eQg1hfG.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

點擊開始使用API

<br>

<img src="https://i.imgur.com/m9JYlSW.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

這邊勾選要注意！勾選完記得要點保存！


<br>

<img src="https://i.imgur.com/iS7DPag.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>




接著點入 `Line Developers`



<br>

<img src="https://i.imgur.com/enS3T5p.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

這裡會拿到一個 `Channel Secret` ，保留起來等下會用到。

<br>

<img src="https://i.imgur.com/ALdVjlc.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

`Channel Access Token` 也是我們等下會用到的。

---

接著回到`Heroku` ，並點擊setting!

<br>

<img src="https://i.imgur.com/voXlhSF.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

設定Config Variables！


<br>

<img src="https://i.imgur.com/O0RU06e.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>



把剛剛的`ACCESS_TOKEN` 和 `SECRET` 填入！



<br>

<img src="https://i.imgur.com/SLrWnbG.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

往下拉一點你可以找到你的網址，我們要把網址交給我們的Line Bot。

<br>

<img src="https://i.imgur.com/bGg14KM.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

---

接著回到 `Line Developers` 頁面，點擊`EDIT`。!


<br>

<img src="https://i.imgur.com/ZHkFG6c.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

把剛剛的網址後面加上 `callback` ，按下SAVE。

<br>

<img src="https://i.imgur.com/Qw9swR1.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

按下VERIFY，驗證！!


<br>

<img src="https://i.imgur.com/bmIK9UX.jpg" class="col-md-12 col-sm-12 col-xs-12" alt="" align=center/></img>

<br>

這裡不用擔心，沒通過一樣OK
<a href="https://github.com/line/line-bot-sdk-python/issues/37" style="color:blue;">有類似的問題</a>

<br>

<img src="https://i.imgur.com/A5gASfg.jpg" class="col-md-8 col-sm-8 col-xs-12" alt="" align=center/></img>

<br>



