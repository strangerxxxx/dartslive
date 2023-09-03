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
dartslive = Dartslive()
# or
dartslive = Dartslive("mailaddress", "password")
```

### ログインボーナスをもらう

```python
dartslive.get_bonus()
```

### 現在のレートとスタッツを取得する

```python
dartslive.get_player_data()
```

### 最近のプレイデータを取得する

```python
dartslive.get_latest_list()
```

### 当日と前日のプレイデータを取得する

```python
dartslive.get_player_data()
```
