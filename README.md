# dartslive

DARTSLIVEのサイトからスタッツなどを取得します。

## インストール

以下のコマンドを実行します。

```bash
git clone https://github.com/strangerxxxx/dartslive.git
cd dartslive
pip install -r requirements.txt
```

## 使い方

### 初期化

```python
dl = Dartslive()
# or
dl = Dartslive("mailaddress", "password")
```

### ログインボーナスをもらう

```python
dl.get_bonus()
```

ログインボーナスを入手したかbool値で返します。

### 現在のレートとスタッツを取得する

```python
dl.get_player_data()
```

`(レート, 01スタッツ, クリケットスタッツ)`を返します。

### 最近のプレイデータを取得する

```python
dl.get_latest_list()
```

Generatorで、`(日付, ゲーム種別, スタッツ)`を返します。

### 当日と前日のプレイデータを取得する

```python
dl.get_playdata()
```

Generatorで、`(日付, ゲーム種別, スタッツ)`を返します。
