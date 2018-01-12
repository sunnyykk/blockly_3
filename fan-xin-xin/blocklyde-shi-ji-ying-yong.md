**Blockly的实际应用**

在课堂中我学会了运用Blockly来解决简单的算法问题，接下来便将运用Blockly来对π/4在误差范围内进行近似求值。

首先要知道π/4近似等于1-1/3+1/5-1/7+……+（-1）^\(x+1\)·\[1/（2x+1）\]。

注：因为此程序中的初始赋值为1，所以将通项改为（-1\)^x·\[1/\(2x+10\]。![](/assets/图片2.png)

**XML代码：&lt;xml xmlns="**\[[http://www.w3.org/1999/xhtml"&gt\]\(http://www.w3.org/1999/xhtml"&gt\)\*\*](http://www.w3.org/1999/xhtml"&gt]%28http://www.w3.org/1999/xhtml"&gt%29**);  
\*\*

&lt;variables&gt;

```
&lt;variable id="ebV92L\#%auU\)JspR{3\[9" type=""&gt;x&lt;/variable&gt;

&lt;variable id="}fGdqrSohSlCbR.b$P1F" type=""&gt;y&lt;/variable&gt;
```

&lt;/variables&gt;

&lt;block id="{@-\]qI\*vKQmn7A@Dz$;i" type="variables\_set" x="-87" y="-38"&gt;

    &lt;field id="ebV92L\#%auU\)JspR{3\[9" name="VAR" variableType=""&gt;x&lt;/field&gt;

    &lt;value name="VALUE"&gt;

      &lt;block id="-@YEGLWt2.iat\|Tp.1Zv" type="math\_number"&gt;

        &lt;field name="NUM"&gt;1&lt;/field&gt;

      &lt;/block&gt;

    &lt;/value&gt;

    &lt;next&gt;

      &lt;block id="K\`2P!I\|nfC\#MWg\`zf-AM" type="variables\_set"&gt;

        &lt;field id="}fGdqrSohSlCbR.b$P1F" name="VAR" variableType=""&gt;y&lt;/field&gt;

        &lt;value name="VALUE"&gt;

          &lt;block id="fQ?{.5eAR{:nPZU\]s=SJ" type="math\_number"&gt;

            &lt;field name="NUM"&gt;1&lt;/field&gt;

          &lt;/block&gt;

        &lt;/value&gt;

        &lt;next&gt;

          &lt;block id="o\#dlXpbL\#:argV8VsG3\|" type="controls\_if"&gt;

            &lt;mutation else="1" /&gt;

            &lt;value name="IF0"&gt;

              &lt;block id="Zxr}\(=H\`\*KpSW~q\(gaEI" type="logic\_compare"&gt;

                &lt;field name="OP"&gt;LT&lt;/field&gt;

                &lt;value name="A"&gt;

                  &lt;block id="5UjH\#9bf4t3w$%\|xQ\`=c" type="math\_arithmetic"&gt;

                    &lt;field name="OP"&gt;POWER&lt;/field&gt;

                    &lt;value name="A"&gt;

                      &lt;shadow id="$3:\[N1=\[E=YYm1QgP{DI" type="math\_number"&gt;

                        &lt;field name="NUM"&gt;1&lt;/field&gt;

                      &lt;/shadow&gt;

                      &lt;block id="--LzQ;Xg8K/xFVdv-^rO" type="variables\_get"&gt;

                        &lt;field id="}fGdqrSohSlCbR.b$P1F" name="VAR" variableType=""&gt;y&lt;/field&gt;

                      &lt;/block&gt;

                    &lt;/value&gt;

                    &lt;value name="B"&gt;

                      &lt;shadow id="\(\|;FPVvqcwanzdk\|GCO;" type="math\_number"&gt;

                        &lt;field name="NUM"&gt;1&lt;/field&gt;

                      &lt;/shadow&gt;

                      &lt;block id="f-tU^\_\|x\]e1\]!9;\)PST8" type="math\_arithmetic"&gt;

                        &lt;field name="OP"&gt;DIVIDE&lt;/field&gt;

                        &lt;value name="A"&gt;

                          &lt;shadow id="bqSvO\`N\|E\*hq7{Cp~Iqo" type="math\_number"&gt;

                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                          &lt;/shadow&gt;

                          &lt;block id="qL{9aG/;vZN;S\#Ap0\#ES" type="math\_constant"&gt;

                            &lt;field name="CONSTANT"&gt;PI&lt;/field&gt;

                          &lt;/block&gt;

                        &lt;/value&gt;

                        &lt;value name="B"&gt;

                          &lt;shadow id="UMjBcPa6,\]Y2\*YGuX\[%{" type="math\_number"&gt;

                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                          &lt;/shadow&gt;

                          &lt;block id="9W\[FP\*,9/\`5\|gF\)cDgP!" type="math\_number"&gt;

                            &lt;field name="NUM"&gt;4&lt;/field&gt;

                          &lt;/block&gt;

                        &lt;/value&gt;

                      &lt;/block&gt;

                    &lt;/value&gt;

                  &lt;/block&gt;

                &lt;/value&gt;

                &lt;value name="B"&gt;

                  &lt;block id="L^hQoLujWh.-\*Z,U\]\[kZ" type="math\_number"&gt;

                    &lt;field name="NUM"&gt;0.12&lt;/field&gt;

                  &lt;/block&gt;

                &lt;/value&gt;

              &lt;/block&gt;

            &lt;/value&gt;

            &lt;statement name="DO0"&gt;

              &lt;block id="7~xo^PoqR0Ach\*8Wm2@b" type="text\_print"&gt;

                &lt;value name="TEXT"&gt;

                  &lt;shadow id="{FMJAmDB\(q\*+qD8,8Vo:" type="text"&gt;

                    &lt;field name="TEXT"&gt;abc&lt;/field&gt;

                  &lt;/shadow&gt;

                  &lt;block id="nv{T7@tF,\`2IH/dY=:h/" type="variables\_get"&gt;

                    &lt;field id="}fGdqrSohSlCbR.b$P1F" name="VAR" variableType=""&gt;y&lt;/field&gt;

                  &lt;/block&gt;

                &lt;/value&gt;

              &lt;/block&gt;

            &lt;/statement&gt;

            &lt;statement name="ELSE"&gt;

              &lt;block id="ved\_-!uG7cPDpM,oKL\)M" type="controls\_whileUntil"&gt;

                &lt;field name="MODE"&gt;UNTIL&lt;/field&gt;

                &lt;value name="BOOL"&gt;

                  &lt;block id="e;1CgVq~\|C46tv~JI\*Sg" type="logic\_compare"&gt;

                    &lt;field name="OP"&gt;LT&lt;/field&gt;

                    &lt;value name="A"&gt;

                      &lt;block id="9RQXia4v$Vd=\)i@:nF%\(" type="math\_arithmetic"&gt;

                        &lt;field name="OP"&gt;MINUS&lt;/field&gt;

                        &lt;value name="A"&gt;

                          &lt;shadow id="@@\[-\*B00%mlP:\*J\]c@nS" type="math\_number"&gt;

                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                          &lt;/shadow&gt;

                          &lt;block id="IK\[U02{s^8dMa4N\|hsu3" type="variables\_get"&gt;

                            &lt;field id="}fGdqrSohSlCbR.b$P1F" name="VAR" variableType=""&gt;y&lt;/field&gt;

                          &lt;/block&gt;

                        &lt;/value&gt;

                        &lt;value name="B"&gt;

                          &lt;shadow id="\*\]pIQyl:p4,PM:Sye\]bL" type="math\_number"&gt;

                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                          &lt;/shadow&gt;

                          &lt;block id="\|P8.UCoO$\`Qh!T\]I,Kp\`" type="math\_arithmetic"&gt;

                            &lt;field name="OP"&gt;DIVIDE&lt;/field&gt;

                            &lt;value name="A"&gt;

                              &lt;shadow id="WKxWQQb/L/\`Ecm+4P9l1" type="math\_number"&gt;

                                &lt;field name="NUM"&gt;1&lt;/field&gt;

                              &lt;/shadow&gt;

                              &lt;block id="}mzm}tBYB28X/t;%.W.." type="math\_constant"&gt;

                                &lt;field name="CONSTANT"&gt;PI&lt;/field&gt;

                              &lt;/block&gt;

                            &lt;/value&gt;

                            &lt;value name="B"&gt;

                              &lt;shadow id="\]\(q6c\_S.O5x2\]\]v{\`E\*Q" type="math\_number"&gt;

                                &lt;field name="NUM"&gt;1&lt;/field&gt;

                              &lt;/shadow&gt;

                              &lt;block id="4e;a-a9v\|x^\)O5~D6\#F0" type="math\_number"&gt;

                                &lt;field name="NUM"&gt;4&lt;/field&gt;

                              &lt;/block&gt;

                            &lt;/value&gt;

                          &lt;/block&gt;

                        &lt;/value&gt;

                      &lt;/block&gt;

                    &lt;/value&gt;

                    &lt;value name="B"&gt;

                      &lt;block id="O.iLXu9qyI?/eg\*JJYbN" type="math\_number"&gt;

                        &lt;field name="NUM"&gt;0.12&lt;/field&gt;

                      &lt;/block&gt;

                    &lt;/value&gt;

                  &lt;/block&gt;

                &lt;/value&gt;

                &lt;statement name="DO"&gt;

                  &lt;block id=";\[PYcuyd/mXT$HuyY\|\*S" type="variables\_set"&gt;

                    &lt;field id="}fGdqrSohSlCbR.b$P1F" name="VAR" variableType=""&gt;y&lt;/field&gt;

                    &lt;value name="VALUE"&gt;

                      &lt;block id="v2YqxEb;UyYOZULRrY\*d" type="math\_arithmetic"&gt;

                        &lt;field name="OP"&gt;ADD&lt;/field&gt;

                        &lt;value name="A"&gt;

                          &lt;shadow id="NZk2$?\)ueE}s5t\)}A6gl" type="math\_number"&gt;

                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                          &lt;/shadow&gt;

                          &lt;block id="yeuaXRuSNI.v3AgdD\`O\[" type="variables\_get"&gt;

                            &lt;field id="}fGdqrSohSlCbR.b$P1F" name="VAR" variableType=""&gt;y&lt;/field&gt;

                          &lt;/block&gt;

                        &lt;/value&gt;

                        &lt;value name="B"&gt;

                          &lt;shadow id="@zGdsvAnQa\*d}.qjY\*w\)" type="math\_number"&gt;

                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                          &lt;/shadow&gt;

                          &lt;block id="t\]qXaWV{/s6qhTaOu$-\_" type="math\_arithmetic"&gt;

                            &lt;field name="OP"&gt;MULTIPLY&lt;/field&gt;

                            &lt;value name="A"&gt;

                              &lt;shadow id="}ZocQC2O\_2RtKAy\`Xz!d" type="math\_number"&gt;

                                &lt;field name="NUM"&gt;1&lt;/field&gt;

                              &lt;/shadow&gt;

                              &lt;block id="8pNVkq\|k\(l,l\_5S88Hy2" type="math\_arithmetic"&gt;

                                &lt;field name="OP"&gt;POWER&lt;/field&gt;

                                &lt;value name="A"&gt;

                                  &lt;shadow id="%9bDe74,a,L\)k4se6\`3q" type="math\_number"&gt;

                                    &lt;field name="NUM"&gt;1&lt;/field&gt;

                                  &lt;/shadow&gt;

                                  &lt;block id="1%q~156\*kR3oO6BtvZ\[\]" type="math\_number"&gt;

                                    &lt;field name="NUM"&gt;-1&lt;/field&gt;

                                  &lt;/block&gt;

                                &lt;/value&gt;

                                &lt;value name="B"&gt;

                                  &lt;shadow id="u\#\#P{SnhZt5\#x{Mx1kOo" type="math\_number"&gt;

                                    &lt;field name="NUM"&gt;1&lt;/field&gt;

                                  &lt;/shadow&gt;

                                  &lt;block id="1nR,VmTfjZW5rzOYV.0F" type="variables\_get"&gt;

                                    &lt;field id="ebV92L\#%auU\)JspR{3\[9" name="VAR" variableType=""&gt;x&lt;/field&gt;

                                  &lt;/block&gt;

                                &lt;/value&gt;

                              &lt;/block&gt;

                            &lt;/value&gt;

                            &lt;value name="B"&gt;

                              &lt;shadow id="~YdgvTk5Z\|0y\)zX7o1+K" type="math\_number"&gt;

                                &lt;field name="NUM"&gt;1&lt;/field&gt;

                              &lt;/shadow&gt;

                              &lt;block id="VdoRM-\`PtK\]uX\*nC6J\*O" type="math\_arithmetic"&gt;

                                &lt;field name="OP"&gt;DIVIDE&lt;/field&gt;

                                &lt;value name="A"&gt;

                                  &lt;shadow id="-;-dNsE~LA:Rnpb}Gh3J" type="math\_number"&gt;

                                    &lt;field name="NUM"&gt;1&lt;/field&gt;

                                  &lt;/shadow&gt;

                                  &lt;block id="\)mb@R-xh\[jFax+$DC?l0" type="math\_number"&gt;

                                    &lt;field name="NUM"&gt;-1&lt;/field&gt;

                                  &lt;/block&gt;

                                &lt;/value&gt;

                                &lt;value name="B"&gt;

                                  &lt;shadow id="+RSL1mmlSrk;Ms\`~UhLb" type="math\_number"&gt;

                                    &lt;field name="NUM"&gt;1&lt;/field&gt;

                                  &lt;/shadow&gt;

                                  &lt;block id="vi$JK%G4p+:\|Tz\]uJN9M" type="math\_arithmetic"&gt;

                                    &lt;field name="OP"&gt;ADD&lt;/field&gt;

                                    &lt;value name="A"&gt;

                                      &lt;shadow id="}GTh?CY3WIk-CrF8.z$\*" type="math\_number"&gt;

                                        &lt;field name="NUM"&gt;1&lt;/field&gt;

                                      &lt;/shadow&gt;

                                      &lt;block id="vvs=~nd\_dc\[-:}EnogC3" type="math\_arithmetic"&gt;

                                        &lt;field name="OP"&gt;ADD&lt;/field&gt;

                                        &lt;value name="A"&gt;

                                          &lt;shadow id="y:fi+/~ov\*h70u8CaHWw" type="math\_number"&gt;

                                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                                          &lt;/shadow&gt;

                                          &lt;block id="FT5\[S\|TgT8DetzG@7kTR" type="math\_number"&gt;

                                            &lt;field name="NUM"&gt;2&lt;/field&gt;

                                          &lt;/block&gt;

                                        &lt;/value&gt;

                                        &lt;value name="B"&gt;

                                          &lt;shadow id="p4dX5Q-\_\#V=w!\#I+\)I@n" type="math\_number"&gt;

                                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                                          &lt;/shadow&gt;

                                          &lt;block id="HGaL!;dy2^IGn40j?Zmg" type="variables\_get"&gt;

                                            &lt;field id="ebV92L\#%auU\)JspR{3\[9" name="VAR" variableType=""&gt;x&lt;/field&gt;

                                          &lt;/block&gt;

                                        &lt;/value&gt;

                                      &lt;/block&gt;

                                    &lt;/value&gt;

                                    &lt;value name="B"&gt;

                                      &lt;shadow id="y9!7nCtX7+}tD717P\#q~" type="math\_number"&gt;

                                        &lt;field name="NUM"&gt;1&lt;/field&gt;

                                      &lt;/shadow&gt;

                                      &lt;block id="rO4U50\`}w6\*%A9sX$hOf" type="math\_number"&gt;

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

                      &lt;block id="pUUVM\[^6b\[?viM8zU%sK" type="variables\_set"&gt;

                        &lt;field id="ebV92L\#%auU\)JspR{3\[9" name="VAR" variableType=""&gt;x&lt;/field&gt;

                        &lt;value name="VALUE"&gt;

                          &lt;block id="Xam~y?Go%:9}::C,g7E-" type="math\_arithmetic"&gt;

                            &lt;field name="OP"&gt;ADD&lt;/field&gt;

                            &lt;value name="A"&gt;

                              &lt;shadow id="C+\]W\)\)jq\#\`txL?$$Hs.Y" type="math\_number"&gt;

                                &lt;field name="NUM"&gt;1&lt;/field&gt;

                              &lt;/shadow&gt;

                              &lt;block id="WiVqXRrm+SJ0nr,M\_X\|W" type="variables\_get"&gt;

                                &lt;field id="ebV92L\#%auU\)JspR{3\[9" name="VAR" variableType=""&gt;x&lt;/field&gt;

                              &lt;/block&gt;

                            &lt;/value&gt;

                            &lt;value name="B"&gt;

                              &lt;shadow id=",Q\`O/Nk}xRQFHL^YtjlO" type="math\_number"&gt;

                                &lt;field name="NUM"&gt;1&lt;/field&gt;

                              &lt;/shadow&gt;

                              &lt;block id="}sOi@3P3PF$w\(yDF5B.;" type="math\_number"&gt;

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

                  &lt;block id="0@2\_DvV+I=lXe7{o^2wP" type="text\_print"&gt;

                    &lt;value name="TEXT"&gt;

                      &lt;shadow id="p$0Q\(;oc@}:\`.6npsi2\(" type="text"&gt;

                        &lt;field name="TEXT"&gt;abc&lt;/field&gt;

                      &lt;/shadow&gt;

                      &lt;block id="fkVFH=6SE~;ZE0E\|^zO7" type="variables\_get"&gt;

                        &lt;field id="}fGdqrSohSlCbR.b$P1F" name="VAR" variableType=""&gt;y&lt;/field&gt;

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

首先将初始变量x赋值为1，初始变量y赋值为1，限定误差范围小于0.12，因此如果y-π/4&lt;0.12,则直接打印出y,否则执另一个命令，即进入循环结构。赋值y到y+（-1）^x·\[1/\(2x+1\)\],赋值x到x+1，重复直到y-π/4&lt;0.12。打印y，此时输出的y值即为π/4的近似值。

以下便是运算结果。![](/assets/图片1.png)

