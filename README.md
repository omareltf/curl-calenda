# curl-calenda

Questo repository fornisce un'Azione per interagire con il sito web calenda.it utilizzando il comando `curl`. Da qui il nome `curl calenda`.

## Caratteristiche
- Recupera mensilmente i contenuti da calenda.it
- Leggero e facile da usare

## Disclaimer
This project is for educational purposes only and is not affiliated with calenda.it.

```
$$$$$$$$$$$$$$$$$$$$$$$$$$@@@@@@@@@@@@@@@@$@@@$$$$$$$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$$$WZYnf/ff1txvz0pam&@$$$$$$$$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$@@@8Z(]][][[}]-]?__+1(1[{)nh@@@@@B@@$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$@@@WJ-_{)(1}+il>??[]_-{}}}1/())f0#&&Wa#&@@$$$$$$$$$$$
$$$$$$$$$$$$$$$$@@#j1){~ii~]))]<i_]]]_?\}-(|(|{|(n0h&BB&8@$$$$$$$$$$$
$$$$$$$$$$$$$@$@Wr{({_>!!!!li}[_-<<?[?-})}<?({\([?](zw*8%@$$$$$$$$$$$
$$$$$$$$$$$$$@@8U\~>iIll!~]<~~]?ili-?]~_]_{]+})}|?_~-|jr0B@$$$$$$$$$$
$$$$$$$$$$$$$@BO\?<!li!li~[[-}-_~>>+____??[)/tt//)_?_+[\uc#@@$$$$$$$$
$$$$$$$$$$$$$Bq|?+<!l!>+__?1]-<~~<+_[)\||fcXXXYXvx}?-]?]/nL&@@$$$$$$$
$$$$$$$$$$$@@o)<><!ii!>+]]-[}1||fuXJJJJQ000L00Q0Lct)[(}[[|rb@@$$$$$$$
$$$$$$$$$$@@#t]_!;<-]{)/rzYCLLOmmmwwmmwwwZZOZOOOQJYtt\\{)}|v#@$$$$$$$
$$$$$$$$$$$8v-?+>[jnzUCQ0OZmOZZmmmmmwwmZZOOOOOOO0LCU\1)[-})\J%$$$$$$$
$$$$$$$$$@@&u?-|jvXYJLQ0OOOO0ZmmmmqppddqmZOO0OOOQQQLz\-_>_?{n%$$$$$$$
$$$$$$$$$$$h{-[nccXYCLLQ0OZZOmmwwqpqddpqwO0QOOO0Q0QQXn1<i>~?f&$$$$$$$
$$$$$$$$$$BU}-|ucczYUJCCCL0O0OZmmwwmwmmmO0000OO0OOOQUn)+~>+?r#B$$$$$$
$$$$$$$$$@Mj]]|uccXXYJCLQ00OZZZmwmmmwwmZO00Q0O0000QCLv(_-~+[n&$$$$$$$
$$$$$$$$$@&X(_/ncczYJCLQOOZwwwwqwwmwqqwmOOOO0QQQQQ0QCU/-?]}jqB$$$$$$$
$$$$$$$$$@BCf_/nuuzJCLL0OZmwpdpdpqpppqqmOO0CQQLLLCLQLCr]~_[n%$$$$$$$$
$$$$$$$$$@#j1~/nxnj|(frcXCQOmwqpdpwZUx/(/jrtruXCJYUJCC/->>~]YB@@$$$$$
$$$$$$$$$$or]<ruj)1(rxj)-+?(u0mppOUYvuvXYzvuxxxnzCCQQJj[>?[}/hB@$$$$$
$$$$$$$$$@8oU}Yr\||({(](\(j1(XZdpwQXXnj|?{}1nvXzzzYCCUu/\?+}Y@$$$$$$$
$$$$$$$$$@@@dvUnrrr(xLX?xOJztuJOZZYZZJQOunQUuYJQOJJJJYv{vzvUm@$$$$$$$
$$$$$$$$$@@@#fJvXXuvvvvcJLLcfuC0QLJQLUYZpwmZ00QZ0LLJJUXjvnOOp@$$$$$$$
$$$$$$$$$$$@&/JcYLUzuvXYYJznxc0w0LQZwwOZmmmOOZmZ0LJCUUYv0mZw0@$$$$$$$
$$$$$$$$$$@@%(JzzULQCLCLLQXzuUZqZ0QOmqppqmmwqwmO0LUUUUXJZqOOL@$$$$$$$
$$$$$$$$$$@@8)UvvzJLL0ZZZZzXcJmdmOO0OkhdpdddwZO0LCYYYYzJ0mUCp@$$$$$$$
$$$$$$$$$$$$$vXvuUC0OmmZOxzYuY0Z0QO0C0CZdbkbpwO0LCLLUXzULCCO@@$$$$$$$
$$$$$$$$$$$$$0juuYCQOmOCUr1}?1nuxuXjzZd0YmddqwZ0LLQQYXzZQCp%@@$$$$$$$
$$$$$$$$$$$$$%ZuncYCQLCCzzvnx\(tuLQ0Q0mmOYOmwm0QLLLCUYwhk&@@$@$$$$$$$
$$$$$$$$$$$$$$WXjjzUJUYcuuvvvYCL00Q0O0Q00ZQ0OO0CLCCJUYw%$$$$$$$$$$$$$
$$$$$$$$$$$$$@%QrfcJCcf)-|tf/jxvnrxuczYjrzJL00QJCCJUXYC&$$$$$$$$$$$$$
$$$$$$$$$$$$$@@hnfvCOZCCYcXJJLQQOmmZZmmZZJJZOQCJCJUzcXJW@$$$$$$$$$$$$
$$$$$$$$$$$$$$@@ZjrzL0YUYzXXUCCLL0ZZZmqppw0OQLCCJYznuXUwB@@$$$$$$$$$$
$$$$$$$$$$$$$$$$@wtjczvcXYYCJYJCQZwpqqqqm0CCUJUJvxtxvUXZh@$$$$$$$$$$$
$$$$$$$$$$$$$$$$@@ojtffuczYJLCOOmwqwqm0O0JXcXXvx/\uXYUJo\|8$$$$$$$$$$
$$$$$$$$$$$$$$$$$$@Bmf(\rnvcULOOZZZmQLCCUcunxf//xXUYUOah)ix&@@$$$$$$$
$$$$$$$$$$$$$$$$$$$@@@k\)\jjuXYUUUUUJUXut/\\/jncYJJQo#hb-ii}#@$$$$$$$
$$$$$$$$$$$$$$$$$$$@@@kj/1)}[{1|\(|t/)(tjrrxvzYJC0*M*obL!ll!<r%@@$$$$
$$$$$$$$$$$$$$$@%WhCt]u(|/)))1111)(/frrxnuzYUJCmMM##okZ_!IIl!i+C&@$$$
$$$$$$$@@$@&dL/<IIli+lZf]t/\|((|/fjrxuczYUCCZaMM#M#okZ?!IIlii!ii~}C#@
$$$$$@MOu1+!llIIII!>,j0C(1ffft//trnvcXUJJ0kMMMMMM#akq+ilIl!iii>>>!!>]
@WC|-~i!llIII;;IIli;:0OOO|{jjrrnvzYUJLXp##MMMMMM*hkZl>!ll!ii>><<<lIll
>ii!lllllI;;;;;Ili;"{mqqqdX}jfnuzUCC0oM###MMMM#akhvi>i!!!ii>>>><<l;II
!!!llllII;;;;;III::lYqbkkaoqj((|tcw######MMM#oahhci>ii!iii>>><>><!;II
!!!llI;;;;;;;;;;:::(ZdQ\}i!l_jf/|Z#**#MMMM##oaaaC!i!!iiiii>>>>>><i;II
!!lII;;;;;;;;;;;;;iUmf([?}I!!i<~__I\#MMM###*ooawliii!!iiiiii>>i>i>l;I
!!l:;;;;;;;;;;;;I,nZZqZJct<l>+-_+>l;lCMM#****omIi!!!!!!iiii>iiii>>!;;
!!!;::;;;;;;;;II;\OmkhbmLr;>+-+>i_zX\+[kM#*oow-ii!!!!!!liii>iiiii>iI;
```