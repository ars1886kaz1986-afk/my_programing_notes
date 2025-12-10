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

## created_at や updated_at の変換方法
```
<time>
    {formatDistanceToNow(new Date(thread.created_at), {
    addSuffix: true, // 何日前という表記になる
    locale: ja, // 日本時間表記
    })}
</time>
```