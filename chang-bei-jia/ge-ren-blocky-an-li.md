**个人Blockly案例**

**案例说明：**

  Blockly作为一种编译系统，本质是基于计算机系统。计算机是20世纪最先进的科学技术发明之一，对人类的生产活动和社会活动产生了极其重要的影响。计算机可以进行数值计算，又可以进行逻辑计算，能够按照程序运行，自动、高速处理海量数据。其中，科学计算器是电子计算器的一种，可进行乘方、开方、指数、对数、三角函数、统计等方面的运算，又称函数计算器。此次Blockly案例将编程来计算指定自然数区间内（初始区间为0--100）3和5的倍数之和。改变程序中控制区间上限的变量i的值，即可实现对一定自然数区间内3和5的倍数之和的计算。

**Blockly截图：**

![](/assets/c.1.JPG)

**运行截图：**

![](/assets/c.2.JPG)

![](/assets/c.3.JPG)

![](/assets/c.4.JPG)



将i值改变，即可得到一定区间内3和5的倍数之和，如指定区间为0--10000：

![](/assets/c.5.JPG)



**运行结果截图**

![](/assets/c.6.JPG)

![](/assets/c.7.JPG)



**XML代码：**

v&lt;xml xmlns="http://www.w3.org/1999/xhtml"&gt;

  &lt;variables&gt;

    &lt;variable type="" id="\#I$Y\`xZ0??r~-\[V;\*RRJ"&gt;n&lt;/variable&gt;

    &lt;variable type="" id="{F\|5zM3tQ\#,~Wf4TvSu1"&gt;sum&lt;/variable&gt;

    &lt;variable type="" id="WK3U\`TT:@szX+}PA\_v9\("&gt;i&lt;/variable&gt;

    &lt;variable type="" id="J\[7PBF\*\|Tu\#x04\#/\*I\_-"&gt;文本&lt;/variable&gt;

  &lt;/variables&gt;

  &lt;block type="text\_print" id="PBRg\[7\|f\)u\[%Zq$@\)V+q" x="88" y="-262"&gt;

    &lt;value name="TEXT"&gt;

      &lt;shadow type="text" id="6,WYAWxMF.%nESb\]O$ht"&gt;

        &lt;field name="TEXT"&gt;abc&lt;/field&gt;

      &lt;/shadow&gt;

      &lt;block type="text" id="C\(N3q\_s@dX?XG9nNen\|!"&gt;

        &lt;field name="TEXT"&gt;欢迎使用！&lt;/field&gt;

      &lt;/block&gt;

    &lt;/value&gt;

    &lt;next&gt;

      &lt;block type="text\_print" id="d\|5x3n=h1!1\#G?kiEUe\("&gt;

        &lt;value name="TEXT"&gt;

          &lt;shadow type="text" id="6,WYAWxMF.%nESb\]O$ht"&gt;

            &lt;field name="TEXT"&gt;abc&lt;/field&gt;

          &lt;/shadow&gt;

          &lt;block type="text" id="ta@pS9/C\|?wIZz0t:Z~l"&gt;

            &lt;field name="TEXT"&gt;操作将运算得到一定自然数区间内3和5的倍数之和&lt;/field&gt;

          &lt;/block&gt;

        &lt;/value&gt;

        &lt;next&gt;

          &lt;block type="text\_print" id="N\|jgdOMO=Ls\(}Sg3CG7d"&gt;

            &lt;value name="TEXT"&gt;

              &lt;shadow type="text" id="4\]Rz;$K\*\`1B2?\[K\)Tud{"&gt;

                &lt;field name="TEXT"&gt;abc&lt;/field&gt;

              &lt;/shadow&gt;

              &lt;block type="text\_prompt\_ext" id="5WIQmqPhLwke6APTfGZO"&gt;

                &lt;mutation type="TEXT"&gt;&lt;/mutation&gt;

                &lt;field name="TYPE"&gt;TEXT&lt;/field&gt;

                &lt;value name="TEXT"&gt;

                  &lt;shadow type="text" id="\]Aio-w{5B\|3O.GLDtUHT"&gt;

                    &lt;field name="TEXT"&gt;abc&lt;/field&gt;

                  &lt;/shadow&gt;

                  &lt;block type="text" id="v;4O\]=sjY!xc\[pk9\]}-e"&gt;

                    &lt;field name="TEXT"&gt;请输入指定区间上限&lt;/field&gt;

                  &lt;/block&gt;

                &lt;/value&gt;

              &lt;/block&gt;

            &lt;/value&gt;

            &lt;next&gt;

              &lt;block type="text\_print" id="ZBS!/Iq\`a786~gL\[nxD3"&gt;

                &lt;value name="TEXT"&gt;

                  &lt;shadow type="text" id="6,WYAWxMF.%nESb\]O$ht"&gt;

                    &lt;field name="TEXT"&gt;abc&lt;/field&gt;

                  &lt;/shadow&gt;

                  &lt;block type="text" id="DJG\_Z\*2}4TmhHF@L-S;\["&gt;

                    &lt;field name="TEXT"&gt;继续操作将运算得到该区间内3和5的倍数之和&lt;/field&gt;

                  &lt;/block&gt;

                &lt;/value&gt;

                &lt;next&gt;

                  &lt;block type="variables\_set" id="oh,45.P\#d1v@GWTr@TI@"&gt;

                    &lt;field name="VAR" id="\#I$Y\`xZ0??r~-\[V;\*RRJ" variabletype=""&gt;n&lt;/field&gt;

                    &lt;value name="VALUE"&gt;

                      &lt;block type="math\_number" id="b\#q=Qdhid7XK@nQras=G"&gt;

                        &lt;field name="NUM"&gt;0&lt;/field&gt;

                      &lt;/block&gt;

                    &lt;/value&gt;

                    &lt;next&gt;

                      &lt;block type="variables\_set" id="6YMC^.WCMQeA+Qk{7isB"&gt;

                        &lt;field name="VAR" id="WK3U\`TT:@szX+}PA\_v9\(" variabletype=""&gt;i&lt;/field&gt;

                        &lt;value name="VALUE"&gt;

                          &lt;block type="math\_number" id=".qymOGvVl@!=S-Q{jagi"&gt;

                            &lt;field name="NUM"&gt;6&lt;/field&gt;

                          &lt;/block&gt;

                        &lt;/value&gt;

                        &lt;next&gt;

                          &lt;block type="variables\_set" id=";\*Fn^@3!n9L5K3EDi!x."&gt;

                            &lt;field name="VAR" id="{F\|5zM3tQ\#,~Wf4TvSu1" variabletype=""&gt;sum&lt;/field&gt;

                            &lt;value name="VALUE"&gt;

                              &lt;block type="math\_number" id="JN!L3-{$P\#PNQUvF\*ZhA"&gt;

                                &lt;field name="NUM"&gt;0&lt;/field&gt;

                              &lt;/block&gt;

                            &lt;/value&gt;

                            &lt;next&gt;

                              &lt;block type="controls\_repeat\_ext" id="K3%cID\[fH\_kmdqW\*+suj"&gt;

                                &lt;value name="TIMES"&gt;

                                  &lt;shadow type="math\_number" id="::-NgPM$:/kE\[RtO7r;z"&gt;

                                    &lt;field name="NUM"&gt;10&lt;/field&gt;

                                  &lt;/shadow&gt;

                                  &lt;block type="variables\_get" id="zAp\*{;zxt:3^TY!{hV.E"&gt;

                                    &lt;field name="VAR" id="WK3U\`TT:@szX+}PA\_v9\(" variabletype=""&gt;i&lt;/field&gt;

                                  &lt;/block&gt;

                                &lt;/value&gt;

                                &lt;statement name="DO"&gt;

                                  &lt;block type="variables\_set" id="O14FK4~.%7?\]{pa,A=Jz"&gt;

                                    &lt;field name="VAR" id="\#I$Y\`xZ0??r~-\[V;\*RRJ" variabletype=""&gt;n&lt;/field&gt;

                                    &lt;value name="VALUE"&gt;

                                      &lt;block type="math\_arithmetic" id="I{826n\#}x1?.S\*K^H$Sn"&gt;

                                        &lt;field name="OP"&gt;ADD&lt;/field&gt;

                                        &lt;value name="A"&gt;

                                          &lt;shadow type="math\_number" id="E9Zr.AS\[\|njwedDJez?@"&gt;

                                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                                          &lt;/shadow&gt;

                                          &lt;block type="variables\_get" id="eBm?}JbP%QxO+Gq03Oy;"&gt;

                                            &lt;field name="VAR" id="\#I$Y\`xZ0??r~-\[V;\*RRJ" variabletype=""&gt;n&lt;/field&gt;

                                          &lt;/block&gt;

                                        &lt;/value&gt;

                                        &lt;value name="B"&gt;

                                          &lt;shadow type="math\_number" id="\_rNR2\)zHmOTms\)IZAu$c"&gt;

                                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                                          &lt;/shadow&gt;

                                          &lt;block type="math\_number" id="Dgxs..rcq^--$Msq8r!\`"&gt;

                                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                                          &lt;/block&gt;

                                        &lt;/value&gt;

                                      &lt;/block&gt;

                                    &lt;/value&gt;

                                    &lt;next&gt;

                                      &lt;block type="controls\_if" id="aEYo:mMG4r3X\#Hx\)\#:!P"&gt;

                                        &lt;value name="IF0"&gt;

                                          &lt;block type="logic\_operation" id="ns\|;:xt$nkpRL{@d;PV7"&gt;

                                            &lt;field name="OP"&gt;OR&lt;/field&gt;

                                            &lt;value name="A"&gt;

                                              &lt;block type="logic\_compare" id="JGD$zzKRHy\`=b,.\_aN0N"&gt;

                                                &lt;field name="OP"&gt;EQ&lt;/field&gt;

                                                &lt;value name="A"&gt;

                                                  &lt;block type="math\_modulo" id="nkEzWoxTn\`1oIGplU-S%"&gt;

                                                    &lt;value name="DIVIDEND"&gt;

                                                      &lt;shadow type="math\_number" id="sh+,R-^\[uE4Z\(J!O\)8:?"&gt;

                                                        &lt;field name="NUM"&gt;64&lt;/field&gt;

                                                      &lt;/shadow&gt;

                                                      &lt;block type="variables\_get" id="hjPdJ1ZkJ-M8uWZFMqU\`"&gt;

                                                        &lt;field name="VAR" id="\#I$Y\`xZ0??r~-\[V;\*RRJ" variabletype=""&gt;n&lt;/field&gt;

                                                      &lt;/block&gt;

                                                    &lt;/value&gt;

                                                    &lt;value name="DIVISOR"&gt;

                                                      &lt;shadow type="math\_number" id="1}sHAfwQDqaK-qnShpUi"&gt;

                                                        &lt;field name="NUM"&gt;3&lt;/field&gt;

                                                      &lt;/shadow&gt;

                                                    &lt;/value&gt;

                                                  &lt;/block&gt;

                                                &lt;/value&gt;

                                                &lt;value name="B"&gt;

                                                  &lt;block type="math\_number" id="rvQ.A^7{M8:J\)u-/T1O6"&gt;

                                                    &lt;field name="NUM"&gt;0&lt;/field&gt;

                                                  &lt;/block&gt;

                                                &lt;/value&gt;

                                              &lt;/block&gt;

                                            &lt;/value&gt;

                                            &lt;value name="B"&gt;

                                              &lt;block type="logic\_compare" id="mv;lhEqSF8hJAEdof,sh"&gt;

                                                &lt;field name="OP"&gt;EQ&lt;/field&gt;

                                                &lt;value name="A"&gt;

                                                  &lt;block type="math\_modulo" id="$4f\|OW!0T\#lO{^{DJbbi"&gt;

                                                    &lt;value name="DIVIDEND"&gt;

                                                      &lt;shadow type="math\_number" id="sh+,R-^\[uE4Z\(J!O\)8:?"&gt;

                                                        &lt;field name="NUM"&gt;64&lt;/field&gt;

                                                      &lt;/shadow&gt;

                                                      &lt;block type="variables\_get" id="}HmOYcdo-~J5Tkvcx\#AL"&gt;

                                                        &lt;field name="VAR" id="\#I$Y\`xZ0??r~-\[V;\*RRJ" variabletype=""&gt;n&lt;/field&gt;

                                                      &lt;/block&gt;

                                                    &lt;/value&gt;

                                                    &lt;value name="DIVISOR"&gt;

                                                      &lt;shadow type="math\_number" id="k\[0}x~:7;4rfD8K0\_rO4"&gt;

                                                        &lt;field name="NUM"&gt;5&lt;/field&gt;

                                                      &lt;/shadow&gt;

                                                    &lt;/value&gt;

                                                  &lt;/block&gt;

                                                &lt;/value&gt;

                                                &lt;value name="B"&gt;

                                                  &lt;block type="math\_number" id="},nVKQ!\*O/w,+UBZxbOb"&gt;

                                                    &lt;field name="NUM"&gt;0&lt;/field&gt;

                                                  &lt;/block&gt;

                                                &lt;/value&gt;

                                              &lt;/block&gt;

                                            &lt;/value&gt;

                                          &lt;/block&gt;

                                        &lt;/value&gt;

                                        &lt;statement name="DO0"&gt;

                                          &lt;block type="variables\_set" id=";XNrfONAx^3G\|1p1\(.NU"&gt;

                                            &lt;field name="VAR" id="{F\|5zM3tQ\#,~Wf4TvSu1" variabletype=""&gt;sum&lt;/field&gt;

                                            &lt;value name="VALUE"&gt;

                                              &lt;block type="math\_arithmetic" id="J.,W\#y\]?\_X;~u\(\_Xx\)N~"&gt;

                                                &lt;field name="OP"&gt;ADD&lt;/field&gt;

                                                &lt;value name="A"&gt;

                                                  &lt;shadow type="math\_number" id="E9Zr.AS\[\|njwedDJez?@"&gt;

                                                    &lt;field name="NUM"&gt;1&lt;/field&gt;

                                                  &lt;/shadow&gt;

                                                  &lt;block type="variables\_get" id="B\]GMr!@7TaFm=B\`%KsGn"&gt;

                                                    &lt;field name="VAR" id="{F\|5zM3tQ\#,~Wf4TvSu1" variabletype=""&gt;sum&lt;/field&gt;

                                                  &lt;/block&gt;

                                                &lt;/value&gt;

                                                &lt;value name="B"&gt;

                                                  &lt;shadow type="math\_number" id="\_rNR2\)zHmOTms\)IZAu$c"&gt;

                                                    &lt;field name="NUM"&gt;1&lt;/field&gt;

                                                  &lt;/shadow&gt;

                                                  &lt;block type="variables\_get" id="{:;v%9~L\[8Fr\)\[.W,Iy,"&gt;

                                                    &lt;field name="VAR" id="\#I$Y\`xZ0??r~-\[V;\*RRJ" variabletype=""&gt;n&lt;/field&gt;

                                                  &lt;/block&gt;

                                                &lt;/value&gt;

                                              &lt;/block&gt;

                                            &lt;/value&gt;

                                          &lt;/block&gt;

                                        &lt;/statement&gt;

                                      &lt;/block&gt;

                                    &lt;/next&gt;

                                  &lt;/block&gt;

                                &lt;/statement&gt;

                                &lt;next&gt;

                                  &lt;block type="text\_print" id=":A7BELYo/\|\_;;7OM42SK"&gt;

                                    &lt;value name="TEXT"&gt;

                                      &lt;shadow type="text" id="6,WYAWxMF.%nESb\]O$ht"&gt;

                                        &lt;field name="TEXT"&gt;abc&lt;/field&gt;

                                      &lt;/shadow&gt;

                                      &lt;block type="text" id="xAUJMGOhy\|t\*}?Zn?H\]d"&gt;

                                        &lt;field name="TEXT"&gt;该区间内3和5的倍数之和为&lt;/field&gt;

                                      &lt;/block&gt;

                                    &lt;/value&gt;

                                    &lt;next&gt;

                                      &lt;block type="text\_print" id="6}i{WZf1n%!\]\*\(A/YE\[s"&gt;

                                        &lt;value name="TEXT"&gt;

                                          &lt;shadow type="text" id="@JKDe\|VGkM\|\#o.;@NS.\("&gt;

                                            &lt;field name="TEXT"&gt;abc&lt;/field&gt;

                                          &lt;/shadow&gt;

                                          &lt;block type="variables\_get" id=",RNz/1+\_S1/7Vrw.@k72"&gt;

                                            &lt;field name="VAR" id="{F\|5zM3tQ\#,~Wf4TvSu1" variabletype=""&gt;sum&lt;/field&gt;

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

                &lt;/next&gt;

              &lt;/block&gt;

            &lt;/next&gt;

          &lt;/block&gt;

        &lt;/next&gt;

      &lt;/block&gt;

    &lt;/next&gt;

  &lt;/block&gt;

&lt;/xml&gt;



