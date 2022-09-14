# keypoints-annotation-tool

## 概要
  AISTダンス動画データベース専用のキーポイントアノテーションツールです。

## 事前準備
- **プログラムのダウンロード**  
  このリポジトリをクローンするか、Zipファイルをダウンロードしてください。
  
- **動画のダウロード**  
  AIST Dance Video DataBaseの公式サイトから動画をダウンロードしてください。  
  https://aistdancedb.ongaaccel.jp/  
  （１つのダンスにつき、c01~c08の8つの動画が対象です）
  
- **データのダウンロード**  
  AIST++の公式サイトからcamerasおよびkeypoints2dのデータをダウンロードしてください。  
  https://google.github.io/aistplusplus_dataset/factsfigures.html
  
- **ファイルの構成**  
  以下の図のようにファイルを置いてください
<pre>
.
|
├─ main.exe .. (メインプログラム)
|
├─ config.json .. (設定ファイル)
|
├─ data .. (AIST++のデータファイル)
|   |
|   ├─ cameras
|   |   ├─ mapping.txt
|   |   |      :
|   |   
|   └─ keypoints2d
|       ├─ gBR_sBM_cAll_d04_mBR0_ch01.pkl
|       |               :
|
├─ gBR_sBM_cAll_d04_mBR0_ch01 (AIST Dance Video DataBase の動画ファイル)
|   ├─ gBR_sBM_c01_d04_mBR0_ch01.mp4
|   |                :
|   └─ gBR_sBM_c08_d04_mBR0_ch01.mp4
|
├─ gBR_sBM_cAll_d04_mBR0_ch02
|              :
</pre>
- AIST Dance Video DataBase の動画データは、ダンスごとにcAllというフォルダを作成し、c01~c08までのmp4動画を入れる
- AIST++のcamerasおよびkeypoints2dはzipを解凍してフォルダごとdataに移動させる
  
## キーポイントの説明
以下の説明を参考に、キーポイントのアノテーションを行ってください。  
  ![画像の説明](Pictures/keypoints_explanation.png)
- Hips ... 骨盤（尾てい骨辺り）
- Spine ... 腰（おへその辺り）
- Chest ... みぞおちの辺り（首と骨盤の中間らへん）
- UpperChest ... 胸部
- Neck ... 首の付け根
- HeadTop ... 頭頂
- Jaw ... あご先
- Shoulder ... 肩、肩甲骨の首側
- Palm ... 手のひらの中心部　※見えている場合のみマーク
- Thumb ... 親指の先端
- FingerTip ... 指全体の先端
- Little ... 小指の先端
- Heel ... かかと（靴の後ろ側）
- Toe ... つま先（親指側）

## アノテーションツールの使い方
- **ツールの起動**

- **キーポイントのアノテーション**

- **カメラの切り替え**

- **フレームの移動**

- **Triangulation**

- **Interpolation**

- **進捗確認**

- **アノテーションデータの保存**
