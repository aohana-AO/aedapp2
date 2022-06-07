# 🏥 松山市AED設置マップ

## 📷 image or gif
![20220607_120601](https://user-images.githubusercontent.com/84378453/172287655-3427d000-229c-422a-a0c0-51bce50b1ffc.gif)

## Overview
愛媛県松山市のオープンデータをもとにfoliumで「AED設置箇所,救急医療機関,松山市の医療機関すべて」の場所をプロットしたleafletの地図を作製。
それをまとめdjangoでwebアプリの形にしました。

## Requirement
### base
- Windows10
- Python3.9
- Django4.0.4
### map
- folium
- leaflet.js
### etc
- feedparser

## Description
- 地図のzoom度合いにより表示されるマーカーを集約し、視認性を向上させた。

- マーカーを押すとpopupが表示され住所や名称、施設内の設置箇所とAED個数を表示する。
![スクリーンショット 2022-06-07 111144](https://user-images.githubusercontent.com/84378453/172280924-53afaf55-927f-4ca9-af26-14577ddaf7ad.png)

- 位置情報ボタンを押すと現在地を表示する。
![スクリーンショット 2022-06-07 105059](https://user-images.githubusercontent.com/84378453/172280727-012fce8b-b8e3-4f43-9e35-349b0542b9d0.png)

- その下のマップ変更ボタンを押すとタイルが変更される。
![スクリーンショット 2022-06-07 105621](https://user-images.githubusercontent.com/84378453/172280668-637f9685-b11e-49a3-b6aa-4de690095fc0.png)

- AED設置マップだけでなく救急医療機関などもマップにプロットした。
![20220607_111627](https://user-images.githubusercontent.com/84378453/172281749-00021536-472d-4a2c-a439-166c3d597fa2.gif)

## Reference
- Markerのiconのマーク
https://chayarokurokuro.hatenablog.com/entry/2020/09/02/212350
https://github.com/domoritz/leaflet-locatecontrol
- leaflet現在地表示
https://kita-note.com/leaflet-plugin-locatecontrol
https://kita-note.com/leaflet-plugin-icon-pulse
- データ不足分の緯度経度情報会得
https://elsammit-beginnerblg.hatenablog.com/entry/2021/07/14/225200
- 地図タイル変更
https://2ndart.hatenablog.com/entry/2021/04/28/164803
https://2ndart.hatenablog.com/entry/2021/04/29/111336
