## 日付操作を簡単にするアプリ

```
npm install date-fns
```

## 使い方
```
import { format } from "date-fns"
format(new Date(), "yyyy-MM-dd")
```

##　日付の加算
```
import { addDays } from "date-fns"
addDays(new Date(), 7)

```

## 日本語表記
```
import { ja } from "date-fns/locale"
format(new Date(), "yyyy年MM月dd日", { locale: ja })

```