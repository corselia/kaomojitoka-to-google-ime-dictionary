# Kaomojitoka to Google IME Dictionary

## Google 日本語入力 へのインポート方法
- 辞書ツール -----> 管理 -----> 新規辞書にインポート

## What's 'KAOMOJITOKA'?
- `KAOMOJITOKA` is Japanese emoticons collection
    - The official site is [here](http://kaomoji.n-at.me/)
    - The repository is [here](https://github.com/tatat/kaomoji.html)
- The official site provides Web API
    - The document is [here](https://github.com/tatat/kaomoji.html/blob/master/README.md)

## What's this app?
- This app enables to convert the raw API response such as `KAOMOJITOKA` to Google IME dictionary format

## How to use
- Very simple to use

### 1. Exec app
```bash
$ ruby kaomojitoka_to_google_ime_dictionary.rb
```

### 2. The dictionary file is created
- You can get `./kaomojitoka_to_google_ime_dictionary.sample.txt`, which is the very Google IME dictionary file (CSV)
- The sample of output file is `kaomojitoka_to_google_ime_dictionary.sample.txt`

![kaomojitoka_to_google_ime_dictionary_01.png](screenshots/kaomojitoka_to_google_ime_dictionary_01.png)

### 3. Import dictionary file to Google IME
- Please import `./kaomojitoka_to_google_ime_dictionary.sample.txt` to Google IME

![kaomojitoka_to_google_ime_dictionary_11.png](screenshots/kaomojitoka_to_google_ime_dictionary_11.png)

![kaomojitoka_to_google_ime_dictionary_12.png](screenshots/kaomojitoka_to_google_ime_dictionary_12.png)

![kaomojitoka_to_google_ime_dictionary_13.png](screenshots/kaomojitoka_to_google_ime_dictionary_13.png)

### 4. Confirm to convert correctly
- When Google IME is on, input `かおもじとか` and try to convert.
- The conversion candidates of Japanese emoticons are shown
- Be good communication :)

![kaomojitoka_to_google_ime_dictionary_21.png](screenshots/kaomojitoka_to_google_ime_dictionary_21.png)

![kaomojitoka_to_google_ime_dictionary_22.png](screenshots/kaomojitoka_to_google_ime_dictionary_22.png)

# Note
- Now [`kaomojitoka_to_google_ime_dictionary.rb`](https://github.com/corselia/kaomojitoka-to-google-ime-dictionary/blob/master/kaomojitoka_to_google_ime_dictionary.rb) is uncomplete code because of [this article (Japanese, sorry)](https://obel.hatenablog.jp/entry/20180610/1528593119)
- So I modify [`kaomojitoka_to_google_ime_dictionary.txt`](https://github.com/corselia/kaomojitoka-to-google-ime-dictionary/blob/master/kaomojitoka_to_google_ime_dictionary.txt) **manually**
- I wanna modify this bug(?)
- **Over 300 Bytes word is not registered correctly**

![kaomojitoka_to_google_ime_dictionary_not_registered.png](screenshots/kaomojitoka_to_google_ime_dictionary_not_registered.png)
- If you wanna add multiple lines characters, should use the clip board tool such as [CLCL](https://www.nakka.com/soft/clcl/)

# LICENSE
- [MIT LICENSE](LICENSE)
