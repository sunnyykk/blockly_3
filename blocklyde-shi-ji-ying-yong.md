  
@font-face{  
font-family:"Times New Roman";  
}  
  
@font-face{  
font-family:"宋体";  
}  
  
@font-face{  
font-family:"Calibri";  
}  
  
@font-face{  
font-family:"Calibri Light";  
}  
  
p.MsoNormal{  
mso-style-name:正文;  
mso-style-parent:"";  
margin:0pt;  
margin-bottom:.0001pt;  
mso-pagination:none;  
text-align:justify;  
text-justify:inter-ideograph;  
font-family:Calibri;  
mso-fareast-font-family:宋体;  
mso-bidi-font-family:'Times New Roman';  
font-size:10.5000pt;  
mso-font-kerning:1.0000pt;  
}  
  
p.p{  
mso-style-name:"普通\\(网站\\)";  
margin:0pt;  
margin-bottom:.0001pt;  
mso-pagination:none;  
text-align:justify;  
text-justify:inter-ideograph;  
font-family:Calibri;  
mso-fareast-font-family:宋体;  
mso-bidi-font-family:'Times New Roman';  
font-size:12.0000pt;  
mso-font-kerning:1.0000pt;  
}  
  
span.msoIns{  
mso-style-type:export-only;  
mso-style-name:"";  
text-decoration:underline;  
text-underline:single;  
color:blue;  
}  
  
span.msoDel{  
mso-style-type:export-only;  
mso-style-name:"";  
text-decoration:line-through;  
color:red;  
}  
@page{mso-page-border-surround-header:no;  
	mso-page-border-surround-footer:no;}@page Section0{  
margin-top:70.8500pt;  
margin-bottom:56.7000pt;  
margin-left:70.8500pt;  
margin-right:56.7000pt;  
size:595.3000pt 841.9000pt;  
layout-grid:15.6000pt;  
}  
div.Section0{page:Section0;}

**Blockly的实际应用**



在课堂中我学会了运用Blockly来解决简单的算法问题，接下来便将运用Blockly来对π/4在误差范围内进行近似求值。



首先要知道π/4近似等于1-1/3+1/5-1/7+……+（-1）^\(x+1\)·\[1/（2x+1）\]。

注：因为此程序中的初始赋值为1，所以将通项改为（-1\)^x·\[1/\(2x+10\]。





![](file:///C:\Users\苬樱\AppData\Local\Temp\ksohtml\wpsF78C.tmp.jpg)



&lt;xml xmlns="http://www.w3.org/1999/xhtml"&gt;

&lt;variables&gt;

&lt;variable id="tS+4~/CLZhvc-\_fBQRD{" type=""&gt;x&lt;/variable&gt;

&lt;variable id="lVq:bzW\`S9hABBOzwEf3" type=""&gt;y&lt;/variable&gt;

&lt;/variables&gt;

&lt;block id="J%65\*y;6Bb}\]O4O8mH\#l" type="variables\_set" x="38" y="13"&gt;

&lt;field id="tS+4~/CLZhvc-\_fBQRD{" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="BHb1fSbj;8H%0{nT-2na" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="4?1Ep4=faO\|620i9z1/\(" type="variables\_set"&gt;

&lt;field id="lVq:bzW\`S9hABBOzwEf3" name="VAR" variableType=""&gt;y&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id=",x?R.X?}Se=VM6=24c?+" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="KN,861vSxO51tNyu\(MPn" type="controls\_if"&gt;

&lt;mutation else="1" /&gt;

&lt;value name="IF0"&gt;

&lt;block id="qVg$Cc!%}5fs^S\[Ym6JW" type="logic\_compare"&gt;

&lt;field name="OP"&gt;LT&lt;/field&gt;

&lt;value name="A"&gt;

&lt;block id="\`iY.\_AjXCG?F4Su$hvVg" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;MINUS&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="1rIKG++3LL3O=/w6cWno" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="Ur~9pYbJ\(YEfK1/2P2t;" type="variables\_get"&gt;

&lt;field id="lVq:bzW\`S9hABBOzwEf3" name="VAR" variableType=""&gt;y&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id=";ySo-~gDX\#E\*}Cd:53YN" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="nq\*pf\(RYw8\(ogHhR,R=j" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;DIVIDE&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="~a+I\`\#$MSj\]dxGXX::~\|" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="0O%WbGVUM\`HM~f;?.,Fe" type="math\_constant"&gt;

&lt;field name="CONSTANT"&gt;PI&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="WmQ/LT6P\#\[C4.%pwxN/l" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="}2$\|%Ayaqsv/yt\`^Pz!N" type="math\_number"&gt;

&lt;field name="NUM"&gt;4&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;block id=".w^{6e5p;:X:WMUh7:\`W" type="math\_number"&gt;

&lt;field name="NUM"&gt;0.12&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;statement name="DO0"&gt;

&lt;block id="zCAobhGj5EbAV\|\|P7,hX" type="text\_print"&gt;

&lt;value name="TEXT"&gt;

&lt;shadow id="j}hXXk1cWb1AHBmV=m~s" type="text"&gt;

&lt;field name="TEXT"&gt;abc&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="$SI\(oq?ukN~Q?6JvlUl{" type="variables\_get"&gt;

&lt;field id="lVq:bzW\`S9hABBOzwEf3" name="VAR" variableType=""&gt;y&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/statement&gt;

&lt;statement name="ELSE"&gt;

&lt;block id="X=Nb:R/Cfh-FF49bk52T" type="controls\_whileUntil"&gt;

&lt;field name="MODE"&gt;UNTIL&lt;/field&gt;

&lt;value name="BOOL"&gt;

&lt;block id="\`o:cF2\#=fm^5AI,^iA\*T" type="logic\_compare"&gt;

&lt;field name="OP"&gt;LT&lt;/field&gt;

&lt;value name="A"&gt;

&lt;block id="MH\]Jna:\(f\*BB0DhSE@eL" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;MINUS&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="1rIKG++3LL3O=/w6cWno" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="t^fO\|d5L!y\)iu\(!OIWeb" type="variables\_get"&gt;

&lt;field id="lVq:bzW\`S9hABBOzwEf3" name="VAR" variableType=""&gt;y&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id=";ySo-~gDX\#E\*}Cd:53YN" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="B8Z}jtjYLLW;Lvq\#:L\#3" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;DIVIDE&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="~a+I\`\#$MSj\]dxGXX::~\|" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="\`^\)\#kbck+IywG7B\#{xiO" type="math\_constant"&gt;

&lt;field name="CONSTANT"&gt;PI&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="WmQ/LT6P\#\[C4.%pwxN/l" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="\[EKKQ\)X\(0AVvUWq.gGt\|" type="math\_number"&gt;

&lt;field name="NUM"&gt;4&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;block id="wf.hO7YUY0?U-C~%W3Yp" type="math\_number"&gt;

&lt;field name="NUM"&gt;0.12&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;statement name="DO"&gt;

&lt;block id="\(\#9gV$F{l\_I3,GNJifrR" type="variables\_set"&gt;

&lt;field id="lVq:bzW\`S9hABBOzwEf3" name="VAR" variableType=""&gt;y&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="%\[2qDj7}\|v4Otk6xO~S}" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;ADD&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="O\)DKIxDRt1\|.c}{}-Yy\)" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="R?4;GuwRD~\({VDbNK\`JX" type="variables\_get"&gt;

&lt;field id="lVq:bzW\`S9hABBOzwEf3" name="VAR" variableType=""&gt;y&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="Rk3VDg2o!.\)W\#Wa}0~H," type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="ikglWrf6bQ\*wlOz\|dH%a" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;MULTIPLY&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="4fptD\*J8,YQFAnce\[Y\`\(" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="?;n1}?3M6$\#q!^Y\]l\)I^" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;POWER&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="B9W\_FG27{48NKW\#w:c/\`" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="A9mH%dS\]~:x?ncVfLV-H" type="math\_number"&gt;

&lt;field name="NUM"&gt;-1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="?EW;B;Pu@?$!9P3J1OJ~" type="math\_number"&gt;

&lt;field name="NUM"&gt;0&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="diBjZ\#ZOFc4lYC-\|O{/U" type="variables\_get"&gt;

&lt;field id="tS+4~/CLZhvc-\_fBQRD{" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="s\)qRM\`ut%F^KQ+wnXcm7" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="x\*}wO^2zejQE-\*,De.%k" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;DIVIDE&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="bTi\#Q~dsLNU^uIHyG\]H~" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="kgG+gw!^lcOdO/7ZF\*EN" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="Yo\(KUO~Dp@\*!$\*GI?\]8." type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id=".\]Y42v\*G\*pF7!yzuP\*Ew" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;ADD&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="P-W\`$tpu1@BhbGw7\#j\`T" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="%065A\[3tYz\#!+=cz//\|d" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;MULTIPLY&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="2e4{45\[/MZm\#PF~vwn8K" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="\_/avKtrdLa\*weyxPlMUj" type="math\_number"&gt;

&lt;field name="NUM"&gt;2&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id=".MHhT06.$41^ItXC9\]\[\*" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="l5aqQ\`\`tgO\(QMHZGjiSN" type="variables\_get"&gt;

&lt;field id="tS+4~/CLZhvc-\_fBQRD{" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="V%lcXzLSn/SQahAkMq=3" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="0NJljiXNmp@k+\(;Q,XA5" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;next&gt;

&lt;block id="u50Tk{q\],1W3KYhvXf}o" type="variables\_set"&gt;

&lt;field id="tS+4~/CLZhvc-\_fBQRD{" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;value name="VALUE"&gt;

&lt;block id="ED\`RUB9T9\|LYjZ3Un\[Z\#" type="math\_arithmetic"&gt;

&lt;field name="OP"&gt;ADD&lt;/field&gt;

&lt;value name="A"&gt;

&lt;shadow id="a?\#.{\(^\`1kvkN\[;Xdp\|Q" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="GXSoXOGL\[\`mXmVQ%zNny" type="variables\_get"&gt;

&lt;field id="tS+4~/CLZhvc-\_fBQRD{" name="VAR" variableType=""&gt;x&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;value name="B"&gt;

&lt;shadow id="@KgHxwV\#@+^U;T@k1b9\|" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="SB:\)YW\`Gu,,\`ENnTj8s\`" type="math\_number"&gt;

&lt;field name="NUM"&gt;1&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/statement&gt;

&lt;next&gt;

&lt;block id="U\_8}?afs0S\#S{eP;X^02" type="text\_print"&gt;

&lt;value name="TEXT"&gt;

&lt;shadow id="j}hXXk1cWb1AHBmV=m~s" type="text"&gt;

&lt;field name="TEXT"&gt;abc&lt;/field&gt;

&lt;/shadow&gt;

&lt;block id="D~P\(y{B/wb\_tInY/;D{1" type="variables\_get"&gt;

&lt;field id="lVq:bzW\`S9hABBOzwEf3" name="VAR" variableType=""&gt;y&lt;/field&gt;

&lt;/block&gt;

&lt;/value&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/statement&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/next&gt;

&lt;/block&gt;

&lt;/xml&gt;



首先将初始变量x赋值为1，初始变量y赋值为1，限定误差范围小于0.12，因此如果y-π/4&lt;0.12,则直接打印出y,否则执另一个命令，即进入循环结构。赋值y到y+（-1）^x·\[1/\(2x+1\)\],赋值x到x+1，重复直到y-π/4&lt;0.12。打印y，此时输出的y值即为π/4的近似值。



以下便是运算结果。

![](file:///C:\Users\苬樱\AppData\Local\Temp\ksohtml\wpsF78D.tmp.jpg)

1���XTS![](/assets/图片1.png)

