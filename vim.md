# vim指令



## 基本輸入指令
```
:w	    存檔
:q!	    不存檔離開
a	    從目前游標之後開始輸入
i	    從目前游標之前開始輸入
o	    從目前游標下行開始輸入
```



## 加速編輯技巧
```
G	    移動到最後一行
8G	    移動到第8行
:8	    移動到第8行(同8G)

0	    移動到該行一開始
$	    移動到該行最末尾

{	    移動到該段落一開始
}	    移動到該段落最末尾

H	    移動到畫面開頭
M	    移動到畫面中間
L	    移動到畫面末尾

D	    刪除游標開始觸到本行結尾
dd	    刪除整行
6,9d        刪除6~9行
5dd	    刪除游標開始的5行

yy	    複製該行
p	    貼上複製的東西到游標之後
P	    貼上複製的東西到游標之前
```



## 搜尋及其他

```
/cfg        搜尋cfg
n           (/cfg 的下一筆)
N           (/cfg 的上一筆)
J           合併目前行與下行
u           undo最後的修改(最後的修改的定義不清楚, 別亂用@@)
Ctrl+r      redo
.           重複上一個動作
%           移動到相對應的(), [], {}等符號
```


## 設定環境
參考: http://wiki.csie.ncku.edu.tw/vim/vimrc


$ vi .vimrc
```
:set nu			顯示行號
:set nonu		關閉行號
:set ai			自動內縮
:set noai		關閉內縮
:set ignorecase		搜尋不分大小寫
:set noignorecase	搜尋區分大小寫(預設)
:set tabstop=4		tab鍵=4空白
:set shiftwidth=4	內縮設定為4個空白
:set cursorline		所在行會有底線
:set mouse=a		可以使用滑鼠點選位置
:set mouse=""		取消滑鼠點選位置的功能
:set expandtab		往後使用tab,都會自動換成空白
:retab			將文中所有tab換成空白
:.retab			將目前這行的tab換成空白
```

---
更新日期: 2017/09/23, TonyCJ
