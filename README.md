# mvids_motercycle_signUp

## Introduction
最近朋友開始搶機車駕照，所以就幫忙寫惹

## Depndencies
* requests
* bs4 
* lxmllxml

## Usage 
1. 下載到電腦
 ```shell
 git clone https://github.com/mhy1264/mvdis_bot.git
 ```
 
2. 安裝套件
```
pip install requests bs4 lxml
```

3. 新增 accounts.ini 存放個人基本資料、LineNotifyToken 的檔案，格式如下:<br>
Line Notify Token 可以參考 : [自建 LINE Notify 訊息通知](https://www.oxxostudio.tw/articles/201806/line-notify.html)
```
[Default]
id = 身份證字號
birth = YYYMMDD (YYY是民國年)
name = 姓名
phone = 電話
email = 電子信箱
token = LineNotifyToken
```

4. 更改 監理所(站)代碼


|臺北市區監理所（含金門馬祖）|20|
|---|---|
|士林監理站|21|
|基隆監理站|25|
|金門監理站|26|

|臺北區監理所（北宜花）|40|
|---|---|
|臺北區監理所|40|
|板橋監理站|41|
|宜蘭監理站|43|
|花蓮監理站|44|
|玉里監理分站|45|
|蘆洲監理站|46|

|新竹區監理所（桃竹苗）|50|
|---|---|
|新竹區監理所|50|
|新竹市監理站|51|
|桃園監理站|52|
|中壢監理站|53|
|苗栗監理站|54|

|臺中區監理所（中彰投）|60|
|---|---|
|臺中區監理所|60|
|臺中市監理站|61|
|埔里監理分站|62|
|豐原監理站|63|
|彰化監理站|64|
|南投監理站|65|

|嘉義區監理所（雲嘉南）|70|
|---|---|
|嘉義區監理所|70|
|東勢監理分站|71|
|雲林監理站|72|
|新營監理站|73|
|臺南監理站|74|
|麻豆監理站|75|
|嘉義市監理站|76|

|高雄市區監理所|30|
|---|---|
|高雄市區監理所|30|
|苓雅監理站|31|
|旗山監理站|33|

|高雄區監理所（高屏澎東）|80|
|---|---|
|高雄區監理所|80|
|臺東監理站|81|
|屏東監理站|82|
|恆春監理分站|83|
|澎湖監理站|84|



```python
self.location[60,64] # 這裡的60 是監理站的代碼 64是監理所的代碼
```

5. 執行
```
python mvids.py
```
> **Warning** <br>
> 請斟酌使用本機器人程式，並自行負責使用後所造成的損失!
