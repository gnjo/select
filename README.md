# select
```

select($$$,title,foot).type('type9').pad(6).pos(x,y,number)
 .key()
 .draw(strflg)
 .get(strflg)

+:FIG--------------+
|*sys0 *sys1 *sys2 |
| sys3  sys4  sys5 |
| sys6  sys7  sys8 |
+:help pad*3ring---+

+:FIG--------------+
|*sys0             |
|                  |
|                  |
+:help pad*3ring---+

```
```
32x24
枠を含めると30x20しか入らない。
//width 30rings border2
head_1
body_22 line20 border2
foot_1
```
```
メッセージボックスは一つで足りる。
center select
+-----------------------------+
|select one              01/02|
|                             |
|*yes                        *|
| no                          |
|:                            |
+-----------------------------+

slot>{$data},{$title}
mes>{$data},{$name}
yon>{$title},y //y is first select
sel>{$data},{$title},n //n is first select
len=30;
```

```
let cursor='*',capture='*'
superselect(data,cursor,capture).key(^v<>);
.set(x,y,value)
let data=`
*あ *い *う *え *お
*あ *い *う *え *お
*あ *い *う *え *お
*あ *い *う *え *お
*あ *い *う *え *お
`


```







