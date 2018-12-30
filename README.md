# img_data_gen

Increasing Image by OpenCV

OpenCVと水増しパターンを利用して画像ファイルを水増しします。

対象となる画像のうち2割程度をテスト用に退避したうえで
左右反転、閾値処理、平滑化処理を用いて画像を水増しします。

## 環境

* Windows 10 x64 1809
* Python 3.7.1 x64
* Power Shell 6 x64
* Visual Studio Code x64
* Git for Windows x64

## 構築

プロジェクトを clone してディレクトリに移動します。

```powershell
> git clone https://github.com/kerobot/img_data_gen.git img_data_gen
> cd img_data_gen
```

プロジェクトのための仮想環境を作成して有効化します。

```powershell
> python -m venv venv
> .\venv\Scripts\activate.ps1
```

念のため、仮想環境の pip をアップグレードします。

```powershell
> python -m pip install --upgrade pip
```

依存するパッケージをインストールします。

```powershell
> pip install -r requirements.txt
```

## 実行

face_imageディレクトリに画像ファイルを配置して実行します。

> 画像ファイルごとにテスト用の画像と水増しした画像を出力

```powershell
> python .\img_data_gen.py
```
