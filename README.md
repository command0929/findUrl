> # 링크 감지 v4
>
> 현재 버전 : v4 ( latest )
>
> # 패치노트
>
> Github upload
>
> IP & 한글 주소 뒤 파일 위치까지 지원
>
> 단독 제작
>
> # example.js
>
> ```js
>const findUrl = require("findUrl");
>
>
> function response(room, msg, sender, isGroupChat, replier, imageDB, packageName) {
> 
> const data = findUrl(msg);
>
> if(0 < data.length) replier.reply("《  URL detect v4 》" + "\u200b".repeat(500) + "\n\n" + data.map(e => "url : " + e.url + " ( " + e.title + " )").join("\n"));
>
> }
> ```
