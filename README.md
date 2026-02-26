# curl-calenda

This repository provides a workflow to interact with the website calenda.it using the `curl` command, hence the name `curl calenda`

## Features
- Automatically fetches content from calenda.it


## Disclaimer
This project is for educational purposes only and is not affiliated with calenda.it.

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$@$@@$@@@@$$@$@@$@$@$$$@$@$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$W*W&wOULaB@@B*MBa*@$$@$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$$@$$$$Mc}~]][[}[_-}]]?}\1])tfJtkB@$@@$$$$@$$@$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$@@@@Jn<!~~__?}jr|1+~_+-?<~)uj}1-{{#@@@$@&M@$$$@$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$@@@t!+{/|)\)]~ilI>_-?]_??}|]f{-?|||\(\C*88%Mdhh@$$@$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$@@W[?1n{+<<+?)(|]->I_{_}}_]}n?i/\1)f}1{\cZqh&B@BWB$@$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$%/_)}]~ii!lI;I_}{?]]i>]{{?_+|(?<{x}(n)[[]}(pM%@@@8$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$@C1x+<>l!!i!~>i>li{-~_~~+_?[<<{+]x?[||}/(?-><}fnx0k@@$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$@@@f\_i<>!;!>:~[}_??___i;l~~?-+<])>-[(~]?\>t]~~-i~\xux8@$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$@$Bn/[~<>!l!ll>+}-{i)-_+>>>>_+-+?-??}|)\rjfff/?~[]~+{/cfd$@$$$$$$$$$$$
$$$$$$$$$$$$$$$$$@z(]~~<<!!!~?++-{t??>~<ii<++?[)1([|vzzXcnJvvv|-_-{<][rjUa$@$$$$$$$$$$
$$$$$$$$$$$$$$@$@U?ill<><<i~_{([]]{}(1[[}})fuczczXQLL0OQLQQLJvt(1+?[_?]x|C%$$$$$$$$$$$
$$$$$$$$$$$$$$$@p|][<!!l>+-+-][}(|\tfrcJOmwwwZmmwZZZZOZ00ZOO0Jvx)1j1(?)[\xp@$$$$$$$$$$
$$$$$$$$$$$$$@$8|+{i;I~[|/rrnYJLCOmmOOmmwqwmmmmmmwmmmOOZOOO00UUJ|t\t1)))){0o@$$$$$$$$$
$$$$$$$$$$$$$@Bt++_?>]tuuzUJQ00ZZZmOZZZmZZmmmwwwwmmOOZOOZZZOOLLCU\}1/~]?\1|X%$$$$$$$$$
$$$$$$$$$$$$@@Bj1<+|uvcXYULQ00OOZmOOZmwmwmqmwqpddqwZ0ZQOOOO00QL0Qz(?_?<__?{YB$$$$$$$$$
$$$$$$$$$$$$$$8t<?(ncczXUCQQQQ00ZmOZmwwmwqqppdbdppwmOQ0OOOOQCOQ00Yu/~!>!<?}z%$$$$$$$$$
$$$$$$$$$$$$$@U+]{tczuzzYJLCCQQ0OmZZmmwwqqpdpwppqwmZQ00OZmO0QQ0QQXv/}i~><~~(*$$$$$$$$$
$$$$$$$$$$$$$8([-)fccczXYUJJCJLQ0ZZOZZZmwqwmmqwwwmO0Q0QOOZ0O0ZOQCCxf-_~<!-)tB@$$$$$$$$
$$$$$$$$$$$$$k_?1[rvcccUXXJCJQL0OOmZmZmwwmwOZZwwmOZO000ZOO0OQ0QQLQz/[_?<+_1v8$$$$$$$$$
$$$$$$$$$$$$$Wt|~{xvczcXYUUQC0O0OZqmwwqqwZZZmqwqmZOOZ000Q0QQQQQ00CCn-_[??|upB$$$$$$$$$
$$$$$$$$$$$$$@C(~{xnvnczJLQL0OZ0mwwpddpdpwqqppdpwwmZmZ0mOCLCQCLQQLCv/++-)|z8$$$$$$$$$$
$$$$$$$$$$$$$8t)-}uxjuzYYJYCQQOQZZZppdpbkdpdqwmmJUUcnUzuCLZJUJCLCLLc|><>_[r8@$$$$$$$$$
$$$$$$$$$$$$$d|}<]crnu/[~>>?-[\uULLOwmqpdmQOQcf/\|jvcnnrjcYCJYUJCQQz]~+<i__z8$@$$$$$$$
$$$$$$$$$$$$$m(1l1zur|}1\jcXYn[>~-}rLZwpdOLYccYXxuzzcr\rxxxUcJLCOLUX{{l{1[+J#%$$$$$$$$
$$$$$$$$$$$$@MhQiXvx|((\+xt_<__vn]{1vQqbdqZCUJxz(il[>}zcurYXczUz0CUC\x(l])nC@$$$@$$$$$
$$$$$$$$$$$$$@@hjLur\fx)+[Oc?l>mq{u[vC0wqmQJqXXXpu~~(qX|x0LLCCXUYJJUf{zzfYOO@$$$$$$$$$
$$$$$$$$$$$$$$$@rZvxcvjrrrXU0QQQZOL1rYLOOLLUOJcUJXCCQYCL0m00JCCULUJUv]YuC0Ck@$$$$$$$$$
$$$$$$$$$$$$$@@810nccYUuvvYUUUYJLCjfxU0wZLQQO0LLLCLO0000L0O0OLLQCJCUX(LxQqOk@$$$$$$$$$
$$$$$$$$$$$$$$$BtJczYLCJzzUCUXUYYnxnuLww0QL0mwdqmmZwOO00OZZZQLCCUUJJzzOdOZqZ@$$$$$$$$$
$$$$$$$$$$$$$$$@fvCvXJC0LLQJCQUQJvznXLqqZ0QOZZwqbpwOmqmqqwmO0CCCYUXJcCmkOmO0@$$$$$$$$$
$$$$$$$$$$$$$@$B|rJxzXYLJQQ0OOOOCXUxX0mpmOLOQwdbbpppdpbmZOO0Q0UUXUUzzZULCJCp@$$$$$$$$$
$$$$$$$$$$$$$$$@fnQuucUCQOZmmmwwvUJvC0mhwOmmZCmqbdddbdddpwOOCLUJYYJzYX0JUCY%@$$$$$$$$$
$$$$$$$$$$$$@$$$M(QnvXCL0ZmwmmC/rnrtrL0OOJnuUXLmcOqbkkbpqOZ0QJQQQYzzXLZLOY8$$$$$$$$$$$
$$$$$$$$$$$$$$$$M{YnvXJCQZZZ0UCv//(([tuc(UUCXO0wbOvOpddqwmOQCCQCQYzXXw0CJB@@$$$$$$$$$$
$$$$$$$$$$$$$$$$$hJjxvYCLQ0LLLcXunnx\{\\cQCQ0Q0mOpmn0wqwqQ0QLLLCCUUc%wqB@@@@$$$$$$$$$$
$$$$$$$$$$$$$$$$$$ajjjzUCCLJYzvcvXvzvuccXCJOQZZOZOmZYQwmO0QCLCQCCXJzB$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$@Bfr\nUJCzYxx/txcJQ0ZmZZZwZQJUXYXYQ0QQZ0ZQCLCJCJUYY#$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$@@cjfuXLLYnnn{-+[)1(\\)/jjtt\))rt[|XL0m00LJLQUJYzUXw$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$@#rrfXQOw0CCUYcCOZZZZmmwpbppqwmOwmC0OQZQJCLQCXXvYYO@@$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$mjjnYQOJJJJcYzzXCCJ0COZmZZmwqppqZZO0CQJCCUXcnuzUUh@$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$CrfnYUczYYXUUULJCLCmOwqqqpppqOOQ00LJJJCzcujjvUJnbB$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$@p//rzrxvcUUCLQQOOOwqqwppqmmZ0QJYzXXXYcrt{uXXYCn&-M$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$@$@@t\t/rxvczzYJLQZOmqmqqZmOZOQJzzzzXvj/)fcYXJJxW#i:k$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$@$@$@@()|\rnucXYJ0ZQwZQmZLC0UQYvujurt\\jvXJUYJY&hh+ilo@$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$@$@@X{)|rrnczJYJUUUUJQCJXnt//(|\txucJJJJYWMokk!i!iX$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$@$@$Yx1){}{/juxuxxnxnnrj\\fffrrnvcUJJLzMW#*hw0>!l!iio$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$@$@%z[r|)(){[-??--_-]{\tjrrxnvzXUJJY0MM###apWlilII!!>\@$@$$$$$
$$$$$$$$$$$$$$$$$$@@#0(!l!}|J?|f\(||)))|\\tfrjrxxuvcXUJJLChWM###*opW>>l;Iliiii>?p@$$$$
$$$$$$$$@@$@@@$Mnil!lIIl!} mLj;jtf/|((||\frrxnnczYUUJLYp&M##MMM*hb8;>lI;li>iiiii<+]k$$
$$$$$$$$@8wt<li!lIIIlII!?,>O0J(_rtftt/\/tfnnvzcUUJLYOMMMMMMMM#*hkW;>!lIl!iiii>>>>!li>]
$@$@8U-i>!!!IIIII;;lII!+,`XO0OL})rfrxjfrxucXYUJCLc#MWWMM#MWW#hhk&`>illll!iii><><<lIll!
f?<<>!llllIIIII:;;IIIl>:, pZwmmq11rjrnuuzYJUCCcmMMMMMMMMMM#*hbko,>i!!!!!iii>><><<!IlIl
ii!!!!llllII;;;;;;IIIi:,"1wqbpbphU?r/trncUCLCMM#M#*MMMMWM*akkhk,>ii!!!iii>>>><><<!;III
!!!!llllIII;;;;;I;III::,.Owdkkkaao#[|1{)\)p####*#*MMWM##*hako0ll>ii!iiii>>><<>>><i;III
!!!!!llI;;;;;;;;II;;:::`vOqkbc],' ^"wQcYn#*****#MMMMM##ooahoOIi>liiiiiii>>>>>>>>>>;III
!!!!lI;;;;;;;;II;;;;:;;l0mp_++<-^Ii!i><~~~ O8MWMMMMM***ooaab,ii!iI>i!iii>i>>>>>>>>l;II
!!i;:;I;;;;;;;;;;;I;II'L0QUJcxt]fI!i>~-_--~: u8MMM###***oa*,ii!iiiliii>>ii>>>ii>>>i;II
i!!l";;;;;;;I;;;;I;II^uOwpkdmQUv?I!<--__~>lI+i:*MM#**##*o#:i!i!!!!!l!>iiii>>>>ii>>>I;I
!!!!:,;;;;;I;I;;I;Ill-OqQaakdZLJIl<__~<>i;X0Jj-!(%##**ooM<iii!!!i!i!!I>>ii>ii>iii>>!:;
