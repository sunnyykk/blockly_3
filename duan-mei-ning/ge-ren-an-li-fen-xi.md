**Blockly个人案例报告**

物理科学与技术学院 2017级物理学类1班 段美凝 学号：320170935290

一、案例说明

目的：

利用blockly运算1！+2！+3！+…+n！。

模块截图：

![](/assets/模块（裁剪）.png)

运行方法：

通过改变第一个模块中n的取值（其它模块不变动），以得到n取需要数值时的1！+2！+3！+…+n！的取值。

二、设计过程

设计思路：

先用小循环分别求出1！，2！，3！…，再用大循环把每一项的阶乘加起来，并因为运用了当型结构可以控制加到的范围是1！至输入的n的阶乘。

遇到的困难及解决方案：

1 .个人感到困难的地方是如何把多个“积”加起来（因为两个“积”相加时前一个“积”的数值已被取代），而不影响程序的正常运行。后来采用了增设“和”这一变量的方法，解决了这一问题。

2 .由于设置的变量太多，出现了一些思维混乱。如，没有把每个变量进行赋值，以及小循环结束后忘记将“积”赋值回“1”。所幸后来都找到了错误。

运行结果截图：

1 .输入3之后的结果：

![](/assets/成功1（裁剪）.png)

2 .输入12之后的结果：

![](/assets/成功2（裁剪）.png)

三、XML代码

&lt;xml xmlns="[http://www.w3.org/1999/xhtml"&gt](http://www.w3.org/1999/xhtml"&gt);

&lt;variables&gt;

&lt;variable id="sWbVPkU7\#nKyQ\#?NT5PB" type=""&gt;n&lt;/variable&gt;

&lt;variable id="F\#MtcaH7\#\|TFN,FX-$ZU" type=""&gt;x&lt;/variable&gt;

&lt;variable id="EHa1Y}d?0\#Q/.$X0\#LL\*" type=""&gt;次数&lt;/variable&gt;

&lt;variable id="\_\)Cs\[g9\[\_sctsc\`Y8\#y\]" type=""&gt;积&lt;/variable&gt;

&lt;variable id="So6u3\(;\|M0;0\(3;U7la6" type=""&gt;和&lt;/variable&gt;

&lt;variable id="eHj+L\)j=fJ\(RUJIir\(,}" type=""&gt;a&lt;/variable&gt;

&lt;variable id="\`aEtI:;C\(\|y8tiTMNq\_:" type=""&gt;b&lt;/variable&gt;

&lt;/variables&gt;

&lt;block id="wCAZH$s\]pf+N7MOwE\|O~" type="variables\_set" x="288" y="38"&gt;

&lt;field id="sWbVPkU7\#nKyQ\#?NT5PB" name="VAR" variableType=""&gt;n&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="jt1\|jMi}:5\`48\#uQIR\`=" type="math\_number"&gt;

&lt;field name="NUM"&gt;12&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="\*0h;i:lRZ4tI15}QUI\(\#" type="variables\_set"&gt;

&lt;field id="So6u3\(;\|M0;0\(3;U7la6" name="VAR" variableType=""&gt;和&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="yixJ\_8=O6k5=mT5Zmup0" type="math\_number"&gt;

&lt;field name="NUM"&gt;0&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="!$ci$,ol3wF\)fdMbzibw" type="variables\_set"&gt;

&lt;field id="\_\)Cs\[g9\[\_sctsc\`Y8\#y\]" name="VAR" variableType=""&gt;积&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="g-OTy{\]G!\[$OZ\[iq4P%5" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="\[K,xeEPv\(?i$kEY\*;P9%" type="variables\_set"&gt;

&lt;field id="F\#MtcaH7\#\|TFN,FX-$ZU" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="\`Yps?/\#RzqL9\(sL5f\*Zq" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="xhcwqF\#J+I7kJNG%l.4-" type="controls\_whileUntil"&gt;

&lt;field name="MODE"&gt;WHILE&lt;/field&gt;

&lt;value name="BOOL"&gt;

&lt;block id="f\[m-Ud;Mqv+$+=~jL@\]8" type="logic\_compare"&gt;

&lt;field name="OP"&gt;LTE&lt;/field&gt;

&lt;value name="A"&gt;

&lt;block id="d6Ks2mZWn2YbS\`bZ0W\*m" type="variables\_get"&gt;

&lt;field id="F\#MtcaH7\#\|TFN,FX-$ZU" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;block id="\_@.Bvw?c9Gpnyl89\|uGy" type="variables\_get"&gt;

&lt;field id="sWbVPkU7\#nKyQ\#?NT5PB" name="VAR" variableType=""&gt;n&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;statement name="DO"&gt;

&lt;block id=".p\|eX\*ZBBw?9\_oBV7\`yC" type="variables\_set"&gt;

&lt;field id="EHa1Y}d?0\#Q/.$X0\#LL\*" name="VAR" variableType=""&gt;次数&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="\|f3JkFSc\*U\[!6~\_\(.qVA" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="\#\*+\(yOgPGZCOAEJCY$5Z" type="controls\_whileUntil"&gt;

&lt;field name="MODE"&gt;WHILE&lt;/field&gt;

&lt;value name="BOOL"&gt;

&lt;block id="jj~%-H0BT1s\(V\[=}4pp^" type="logic\_compare"&gt;

&lt;field name="OP"&gt;LTE&lt;/field&gt;

&lt;value name="A"&gt;

&lt;block id=".\*MuvvtDXU-=Q\)oMCq5g" type="variables\_get"&gt;

&lt;field id="EHa1Y}d?0\#Q/.$X0\#LL\*" name="VAR" variableType=""&gt;次数&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;block id="oeIAq:^/?{83%nA6i\|RR" type="variables\_get"&gt;

&lt;field id="F\#MtcaH7\#\|TFN,FX-$ZU" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;statement name="DO"&gt;

&lt;block id="d0\]\|RY\]\*Z9h\`1dF\_08?6" type="variables\_set"&gt;

&lt;field id="\_\)Cs\[g9\[\_sctsc\`Y8\#y\]" name="VAR" variableType=""&gt;积&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="lz\_kozKJ\[p/\]y~^2YWg\|" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;MULTIPLY&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="XP{l+ppPiX\(YEIU\(:p8^" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="mkzPH+{,T\_bm7\(^/h2h4" type="variables\_get"&gt;

&lt;field id="EHa1Y}d?0\#Q/.$X0\#LL\*" name="VAR" variableType=""&gt;次数&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="^IP,wa.6Y\|CX!~6\|\[!Q9" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="cS\|f/,5kGUT@L1W^BD6\`" type="variables\_get"&gt;

&lt;field id="\_\)Cs\[g9\[\_sctsc\`Y8\#y\]" name="VAR" variableType=""&gt;积&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="V~~^2sc4\#fNHS$YBH8TA" type="variables\_set"&gt;

&lt;field id="EHa1Y}d?0\#Q/.$X0\#LL\*" name="VAR" variableType=""&gt;次数&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="\*w5\#x\#nn,yIsOvE4Lj1+" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;ADD&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="jZlxX4ou$HX@XPb-BPB\#" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="aL\`XXhkfOMy\[.RhMD3\)P" type="variables\_get"&gt;

&lt;field id="EHa1Y}d?0\#Q/.$X0\#LL\*" name="VAR" variableType=""&gt;次数&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="/Zlig%\]9!L1a7hv%g?IN" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/statement&gt;

&lt;next&gt;

&lt;block id="Q@N\*,%-P\#he:Zx1L\(\(\[K" type="variables\_set"&gt;

&lt;field id="So6u3\(;\|M0;0\(3;U7la6" name="VAR" variableType=""&gt;和&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="Mtz6Z.\*zqCp:\_uk\)RO\)\]" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;ADD&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="4InrUaMk\)rnU$}JCW!BH" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="438aTn\|s$7hV\_yl3.L1X" type="variables\_get"&gt;

&lt;field id="\_\)Cs\[g9\[\_sctsc\`Y8\#y\]" name="VAR" variableType=""&gt;积&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="z\[A^mrdR\(TxhJm\*y9H^N" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="CX\_$E}\_Fd\|j8VS!a\*-G\*" type="variables\_get"&gt;

&lt;field id="So6u3\(;\|M0;0\(3;U7la6" name="VAR" variableType=""&gt;和&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="X\#ExXW\(E\]\*eyhS+\]OI2{" type="variables\_set"&gt;

&lt;field id="\_\)Cs\[g9\[\_sctsc\`Y8\#y\]" name="VAR" variableType=""&gt;积&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="9H?XGU\_rc\|F\*1u,@UZ8v" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="0:O2dYlmgrfY};epU?-0" type="variables\_set"&gt;

&lt;field id="F\#MtcaH7\#\|TFN,FX-$ZU" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="oRc:\|Jejx;JnK\[p,{Ex." type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;ADD&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="B9T@}w0Q$%:Pj\]OZI7jo" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="+%dFPa\[yAtLnaPV\)a+mm" type="variables\_get"&gt;

&lt;field id="F\#MtcaH7\#\|TFN,FX-$ZU" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="Yj%\_PEvR$vkR\]tXk}tp?" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/statement&gt;

&lt;next&gt;

&lt;block id="P5UVMF\|l$+~yb\#BI@s{9" type="text\_print"&gt;

&lt;value name="TEXT"&gt;

&lt;shadow id=";P,h%HK%u@EJb?m\[MwKl" type="text"&gt;

&lt;field name="TEXT"&gt;abc&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="afIq\*AsGq8\_;%xv^0=h\(" type="variables\_get"&gt;

&lt;field id="So6u3\(;\|M0;0\(3;U7la6" name="VAR" variableType=""&gt;和&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/xml&gt;

