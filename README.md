# curl-calenda

This repository provides a workflow to interact with the website calenda.it using the `curl` command, hence the name `curl calenda`

## Features
- Automatically fetches content from calenda.it


## Disclaimer
This project is for educational purposes only and is not affiliated with calenda.it.

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$@$$$$$@$$$@$$@$$$$$$$$$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$$$$$WmYnj/ff)fncz0dam&@$$$$$$$$$$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$@@8Z(]][][[}]-]?__+1(1]{(uh@$$@@@@$$$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$$WJ-_{)()}+il>??}]_-1}{})/(((jOM&&Wa#8$$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$#j1){~ii~]))]~i-]]]_?\}-||||{|(nOh&BB&8$$$$$$$$$$$$
$$$$$$$$$$$$$$$$Wr1|{_>!i!i!>}[_-<<?}?-{([<]|1\([?[(Xw*8B$$$$$$$$$$$$
$$$$$$$$$$$$$$$8U|+>iIll!+]<~+[?ili-]]~_]_1]_})}(?_~?\jrZB$$$$$$$$$$$
$$$$$$$$$$$$$$BO\?<!!i!l>~}}?}-_~>>+____??})/ttt/)_?_+[/uzM$$$$$$$$$$
$$$$$$$$$$$$$Bw|?+<!l!>+_-]1]-~~~~__})\||jcXXXYXvr}?-]?]tnL8$$$$$$$$$
$$$$$$$$$$$$$*)<<<!ii!>+[[-[}1|\fuYJJJJQ0O0L00Q0Lct)}({[[|rk$$$$$$$$$
$$$$$$$$$$@@#t[_!I~?[{(/xzUCLLOmmmwwwwwwwmZOZOOOQJYtt\\{1}|c#@$$$$$$$
$$$$$$$$$$$8u-?+>}jnzUCQ0OZmOZZmmmmmwwwmZOOOOZOO0LCJ\1)]?})\JB$$$$$$$
$$$$$$$$$$$Wn]-|jvXYJQQ0OOOOOZmmmwqppddqmZOOOOOOQ0QQz\-_<_?1u%$$$$$$$
$$$$$$$$$$$h{-}nccXYCLL00OZZZwmwwqpqddqqwO0QOOO0Q00QYn1>>>~?j8$$$$$$$
$$$$$$$$$$%X}?\vccXYUJCLLL0OOOZmmwwmwmmmO0000OO0OOOQUn)+~>+]x#B$$$$$$
$$$$$$$$$$#f][\uczXYYJLLQ0OZZZZmwmmmwwmZOO00OO0000QCLu(_-~+[u&$$$$$$$
$$$$$$$$$$&X(_/ucczYJCL0ZOmwwwwqwwmwqqwmOOOO0QQQQQ00LUt-?]}rqB$$$$$$$
$$$$$$$$$$BJf_tnuuXCLLQ0ZZmqpdpdpqppppqmZOOCQQLLLCLQQCr]~_}u%$$$$$$$$
$$$$$$$$$$*j)~tnxnj|(jxcYCQOmwpddpwOUx\|/rrfruXCJYJJCC/->>~]UB$$$$$$$
$$$$$$$$$$ar]<xuj)1(rxj)-_](v0mppOUYvvvYYzvuxnxnXCCQQJj[>?[}ta@$$$$$$
$$$$$$$$$$8oU{Yx\||({|]|\|r1(YZddwQYXnj|]{{1nvXzzXYCCJu/\?+}U$$$@$$$$
$$$$$$$$$$$$pvUnrxr|nLz?uZJXtvJOZZYZZC0Ouu0UuUJQ0CJJJUv}vXvJm$$$$$$$$
$$$$$$$$$$$$MjJvXXuvcvvcJLLzfuL00LJQQUUZpwmZ00QZ0QLJJJYjvuOOp$$$$$$$$
$$$$$$$$$$$$&tUcYLUzvcXUYJcnxzOwOLQZwwOmwwmZOZmZ0LCCUUYv0mZwO$$$$$$$$
$$$$$$$$$$$$%|JzXJLQCLLLLQXzuUZwZ00OmqppqwwwqwmZ0LUUUUXJmqOOL@$$$$$$$
$$$$$$$$$$$$8)UvcXCLLOZmZZzXcJmdmOOOOkhdpbddwmO0LCUUYYzC0mULd$$$$$$$$
$$$$$$$$$$$$$cXvuUC0OmmmOxzUuUOZOQO0C0CmbbkbpwZ0LCLLUXzULCLO@@$$$$$$$
$$$$$$$$$$$$$OruuYCQOmOLUr1{?)uuxuXrXZd0UmddqwZ0LLQQYXzmQCpB$$$$$$$$$
$$$$$$$$$$$$$%ZunzYCQQCCczvux\(tvL00Q0mmOYZmqm0QLQLCUYqhh8$$$$$$$$$$$
$$$$$$$$$$$$$$MXjrzUCUYcuuvvvYCL00Q0O0QOOZQ0ZO0CLLCJUYwB$$$$$$$$$$$$$
$$$$$$$$$$$$$$%LrjcJCcf)-\ff/jxvnrxuzzYjrzJLO0QJCCJUXYL%$$$$$$$$$$$$$
$$$$$$$$$$$$$$$hnjvCOZCCYcXJCQQQOmmZZwwZZJJZOQCJLCUzzXJ8$$$$$$$$$$$$$
$$$$$$$$$$$$$$$@ZjrXL0UUYzXXJCCLLOZmZmqppw0ZQLCCJYznuXUqB$$$$$$$$$$$$
$$$$$$$$$$$$$$$$@mtjzzvzYYYCJYJCQZwpqqpqw0CCJJUCvxtxcUXma$$$$$$$$$$$$
$$$$$$$$$$$$$$$$$$ajtffuczYJLLZOwqqwqm0O0JXcXYvx//uXYUJ#\/%$$$$$$$$$$
$$$$$$$$$$$$$$$$$$@Bmf(/ruvcULOOZmZmQQCLUcunnf//nXUYUOah)>n8$$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$@k\)\jjuXUUUJUJJUXut/\\/jncUJJQo#hb-ii1M$$$$$$$$
$$$$$$$$$$$$$$$$$$$$$$kj\))}[{1|\(\f/(|tjrrnvzYJCO*M*obL!ll!~nB@$$$$$
$$$$$$$$$$$$$$$@%WhCf]u|\/(()1111((/frrxnuzYJJCwMM##okm~!IIlii_Q&@$$$
$$$$$$$@$$@&dQ/<IIli+IZj]f/\||(|/fjrxucXYJCLmoMMMM#okO]iII!iiiii~{LM@
$$$$$@WZv)+!llIIII!<"x0C))ffft//fruvzXUJJOhMMMMMM#akm_ilIl!iii>>>!i>[
$WC|-~i!llIII;;IIli;,ZOOO|{jrrxnvzYUJLXd#MMMMMM#*hkZ!i!l!!ii>><<<!Ill
>>i!!lllII;;;;IIli;^{wqppdX}jjnuzJCL0o###MMMMM#akavi>i!!!ii>>>><<l;II
!!!!lllII;;;;;III:,lYqbkko*qj((|tzq######MMM#*ahhciiiiiiii>>><>><!;II
!!!!lII;;;;;;I;;:::|ZdQ/}i!l?rj/\mM**#MMMMM#oaaaJi>!iiiiii>>>>>>>i;II
!!!II;;;;;;;;;;;;;<Jmf(}?}I!!><~__;fMMMMM##*ooawliii!!iii>ii>>>>>>lII
!!l:;;;;;;;;;;III;uZZpZJct<!>+--+<l;!LMM#****owIii!!!!!iii>>iiii>>!II
!i!::;;;;;I;IIII;tOmkabmLr;>+-+<i_YX\+{hM#***m_ii!!!!!!li>i>ii>ii>iI;
