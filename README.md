# Jerry的日記網站

##介紹

因為我想做一個網站，所以就有了這個網站!

##成果展示

![](

## 使用技術

名稱    |    說明
-------|-----------
Python | 不用解釋吧!
Flask  | 幫我架設網站的功臣
repl.it | 線上寫程式環境
Heroku | 免費放網站的佛心公司
Github | 真正的佛心企業

## 範例代碼

```python
@app.route("/")
def root():
  ds = glob.glob("articles/*")
  result = []
  for d in ds:
    fs = glob.glob(d + "/*.txt")
    t = (d.split("/")[-1], len(fs))
    result.append(t)
  return render_template("index.html", d = result)
```

## 網址

[請點我](https://jerry113432.herokuapp.com/)
