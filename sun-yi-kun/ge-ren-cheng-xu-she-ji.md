**《基于机器人的实践方法》个人程序设计报告**  
**2016级计算机基地班 孙逸鲲320160905591**

案例说明：  
程序使用blockly编写。  
功能为：用户从键盘输入一个十进制整数，程序计算出该小于该整数的所有质数。  
由于时间精力能力有限，代码稍显粗浅简陋，望老师多多包涵。

**拼接好的模块截图：**  
 ![](/assets/002.jpg)

**运行结果截图： **  
 ![](/assets/004.jpg)  
 ![](/assets/006.jpg)  
![](/assets/008.jpg)

**XML代码：**

    &lt;xml xmlns="http://www.w3.org/1999/xhtml"&gt;

      &lt;variables&gt;

        &lt;variable type="" id="\]Qv\]t\[GZQthdL8KjpTZW"&gt;m&lt;/variable&gt;

        &lt;variable type="" id="S}kr\[\]{Uy\*DU6$K3uip}"&gt;n&lt;/variable&gt;

        &lt;variable type="" id="K:L-Tq4sa\[H;8i$GkHG\|"&gt;i&lt;/variable&gt;

        &lt;variable type="" id="R?-A9ngC3ib\]+fVv\]3ti"&gt;j&lt;/variable&gt;

        &lt;variable type="" id="tyoreQKzw\_F:U\`O4nL:C"&gt;一个字符串&lt;/variable&gt;

      &lt;/variables&gt;

      &lt;block type="text\_print" id="+luIJrq-B@SeqzTkOEAk" x="-613" y="-38"&gt;

        &lt;value name="TEXT"&gt;

          &lt;shadow type="text" id="dWrZ}!}OH,U8@VZ8d\[xt"&gt;

            &lt;field name="TEXT"&gt;\*\*\*\*功能是输出m以内的质数\*\*\*\*&lt;/field&gt;

          &lt;/shadow&gt;

        &lt;/value&gt;

        &lt;next&gt;

          &lt;block type="variables\_set" id="\|J~49v\*@Q\)pe.MfnQvBh"&gt;

            &lt;field name="VAR" id="\]Qv\]t\[GZQthdL8KjpTZW" variabletype=""&gt;m&lt;/field&gt;

            &lt;value name="VALUE"&gt;

              &lt;block type="text\_prompt\_ext" id="\`}\]\*,Tr9qZzeM416:xIL"&gt;

                &lt;mutation type="TEXT"&gt;&lt;/mutation&gt;

                &lt;field name="TYPE"&gt;TEXT&lt;/field&gt;

                &lt;value name="TEXT"&gt;

                  &lt;shadow type="text" id="=\*O+$dmE.n^R\_$\*{7\*@4"&gt;

                    &lt;field name="TEXT"&gt;请输入数字m&lt;/field&gt;

                  &lt;/shadow&gt;

                &lt;/value&gt;

              &lt;/block&gt;

            &lt;/value&gt;

            &lt;next&gt;

              &lt;block type="variables\_set" id="+}6^G\[bVkRaHPPQ\*{!\*\_"&gt;

                &lt;field name="VAR" id="tyoreQKzw\_F:U\`O4nL:C" variabletype=""&gt;一个字符串&lt;/field&gt;

                &lt;value name="VALUE"&gt;

                  &lt;block type="variables\_get" id="aIWwnH}=8ez9}Bf,\_fO+"&gt;

                    &lt;field name="VAR" id="\]Qv\]t\[GZQthdL8KjpTZW" variabletype=""&gt;m&lt;/field&gt;

                  &lt;/block&gt;

                &lt;/value&gt;

                &lt;next&gt;

                  &lt;block type="text\_append" id="Y.uvR\|CxUAg=%wVeQg0A"&gt;

                    &lt;field name="VAR" id="tyoreQKzw\_F:U\`O4nL:C" variabletype=""&gt;一个字符串&lt;/field&gt;

                    &lt;value name="TEXT"&gt;

                      &lt;shadow type="text" id="cy:M1+;a\]pzNe@xbQ%~="&gt;

                        &lt;field name="TEXT"&gt;&lt;/field&gt;

                      &lt;/shadow&gt;

                      &lt;block type="text" id="=\]yZt/\*\(D;\|tG3\`0-~A,"&gt;

                        &lt;field name="TEXT"&gt;以内的质数有： &lt;/field&gt;

                      &lt;/block&gt;

                    &lt;/value&gt;

                    &lt;next&gt;

                      &lt;block type="controls\_for" id="g4Xm?O;t/aJdv\];\|rC=@"&gt;

                        &lt;field name="VAR" id="K:L-Tq4sa\[H;8i$GkHG\|" variabletype=""&gt;i&lt;/field&gt;

                        &lt;value name="FROM"&gt;

                          &lt;shadow type="math\_number" id="T-soLurgWiH1TWsn\[gRA"&gt;

                            &lt;field name="NUM"&gt;2&lt;/field&gt;

                          &lt;/shadow&gt;

                        &lt;/value&gt;

                        &lt;value name="TO"&gt;

                          &lt;shadow type="math\_number" id="~K\`KSINl-\(x!~NmoV~\(d"&gt;

                            &lt;field name="NUM"&gt;10&lt;/field&gt;

                          &lt;/shadow&gt;

                          &lt;block type="variables\_get" id="prvHTc\*pEA\)d6MKrhZmg"&gt;

                            &lt;field name="VAR" id="\]Qv\]t\[GZQthdL8KjpTZW" variabletype=""&gt;m&lt;/field&gt;

                          &lt;/block&gt;

                        &lt;/value&gt;

                        &lt;value name="BY"&gt;

                          &lt;shadow type="math\_number" id="$Ql\*p@UPpy7nKoq!Hw52"&gt;

                            &lt;field name="NUM"&gt;1&lt;/field&gt;

                          &lt;/shadow&gt;

                        &lt;/value&gt;

                        &lt;statement name="DO"&gt;

                          &lt;block type="controls\_for" id="uj7G/09b6hcUEQ,\[i?8D"&gt;

                            &lt;field name="VAR" id="S}kr\[\]{Uy\*DU6$K3uip}" variabletype=""&gt;n&lt;/field&gt;

                            &lt;value name="FROM"&gt;

                              &lt;shadow type="math\_number" id="G\]uBrEANvuc+FET\]/anB"&gt;

                                &lt;field name="NUM"&gt;2&lt;/field&gt;

                              &lt;/shadow&gt;

                            &lt;/value&gt;

                            &lt;value name="TO"&gt;

                              &lt;shadow type="math\_number" id="^l\[H;iUN15k6TWoQk1NZ"&gt;

                                &lt;field name="NUM"&gt;10&lt;/field&gt;

                              &lt;/shadow&gt;

                              &lt;block type="math\_arithmetic" id="-FY0elR0e!;e5;2hcog."&gt;

                                &lt;field name="OP"&gt;MINUS&lt;/field&gt;

                                &lt;value name="A"&gt;

                                  &lt;shadow type="math\_number" id="XDe/o\($JQJWPf+QS{F;!"&gt;

                                    &lt;field name="NUM"&gt;1&lt;/field&gt;

                                  &lt;/shadow&gt;

                                  &lt;block type="variables\_get" id="gixwgk2\)KC4\#iwL1@IuJ"&gt;

                                    &lt;field name="VAR" id="\]Qv\]t\[GZQthdL8KjpTZW" variabletype=""&gt;m&lt;/field&gt;

                                  &lt;/block&gt;

                                &lt;/value&gt;

                                &lt;value name="B"&gt;

                                  &lt;shadow type="math\_number" id=".YVAxL{5/v==VsVh\`o\*+"&gt;

                                    &lt;field name="NUM"&gt;1&lt;/field&gt;

                                  &lt;/shadow&gt;

                                &lt;/value&gt;

                              &lt;/block&gt;

                            &lt;/value&gt;

                            &lt;value name="BY"&gt;

                              &lt;shadow type="math\_number" id="yPOb\[X,8!\(r5FJCWwBQ="&gt;

                                &lt;field name="NUM"&gt;1&lt;/field&gt;

                              &lt;/shadow&gt;

                            &lt;/value&gt;

                            &lt;statement name="DO"&gt;

                              &lt;block type="controls\_if" id="}^Y\|o@^}pgV+Luu0N7\]E"&gt;

                                &lt;value name="IF0"&gt;

                                  &lt;block type="logic\_compare" id="krR/^/\*MLOC@SGY5QXl3"&gt;

                                    &lt;field name="OP"&gt;EQ&lt;/field&gt;

                                    &lt;value name="A"&gt;

                                      &lt;block type="math\_modulo" id="n9Qc^SNJ+=!1p\#+!z5y7"&gt;

                                        &lt;value name="DIVIDEND"&gt;

                                          &lt;shadow type="math\_number" id="?\*f.VJ\]EuLIPKA890%ca"&gt;

                                            &lt;field name="NUM"&gt;64&lt;/field&gt;

                                          &lt;/shadow&gt;

                                          &lt;block type="variables\_get" id="npApH2s\[l4D5+\_\)\|eY3/"&gt;

                                            &lt;field name="VAR" id="K:L-Tq4sa\[H;8i$GkHG\|" variabletype=""&gt;i&lt;/field&gt;

                                          &lt;/block&gt;

                                        &lt;/value&gt;

                                        &lt;value name="DIVISOR"&gt;

                                          &lt;shadow type="math\_number" id="Z?.K\#=Isv;7gSBW~+hZ2"&gt;

                                            &lt;field name="NUM"&gt;10&lt;/field&gt;

                                          &lt;/shadow&gt;

                                          &lt;block type="variables\_get" id=";2n3q\)@=:V;\[t@kdL2B6"&gt;

                                            &lt;field name="VAR" id="S}kr\[\]{Uy\*DU6$K3uip}" variabletype=""&gt;n&lt;/field&gt;

                                          &lt;/block&gt;

                                        &lt;/value&gt;

                                      &lt;/block&gt;

                                    &lt;/value&gt;

                                    &lt;value name="B"&gt;

                                      &lt;block type="math\_number" id="=%?g8DuVz4PUvYs;0Af%"&gt;

                                        &lt;field name="NUM"&gt;0&lt;/field&gt;

                                      &lt;/block&gt;

                                    &lt;/value&gt;

                                  &lt;/block&gt;

                                &lt;/value&gt;

                                &lt;statement name="DO0"&gt;

                                  &lt;block type="controls\_flow\_statements" id="x:AMyEM}6gH\(B-Y0t=j8"&gt;

                                    &lt;field name="FLOW"&gt;BREAK&lt;/field&gt;

                                  &lt;/block&gt;

                                &lt;/statement&gt;

                              &lt;/block&gt;

                            &lt;/statement&gt;

                            &lt;next&gt;

                              &lt;block type="controls\_if" id=",P/^nG,X.C}y0c9ZZvT/"&gt;

                                &lt;value name="IF0"&gt;

                                  &lt;block type="logic\_compare" id="\_MKW,Bg,O3ea:1aHqb1="&gt;

                                    &lt;field name="OP"&gt;EQ&lt;/field&gt;

                                    &lt;value name="A"&gt;

                                      &lt;block type="variables\_get" id="\`=5U-\_JSzAkxaz.-X\`9q"&gt;

                                        &lt;field name="VAR" id="K:L-Tq4sa\[H;8i$GkHG\|" variabletype=""&gt;i&lt;/field&gt;

                                      &lt;/block&gt;

                                    &lt;/value&gt;

                                    &lt;value name="B"&gt;

                                      &lt;block type="variables\_get" id="A-@%40\*qBfdT7\#q/JLRz"&gt;

                                        &lt;field name="VAR" id="S}kr\[\]{Uy\*DU6$K3uip}" variabletype=""&gt;n&lt;/field&gt;

                                      &lt;/block&gt;

                                    &lt;/value&gt;

                                  &lt;/block&gt;

                                &lt;/value&gt;

                                &lt;statement name="DO0"&gt;

                                  &lt;block type="text\_append" id="u6lqCQLI\)d\#N9y@:\]U8p"&gt;

                                    &lt;field name="VAR" id="tyoreQKzw\_F:U\`O4nL:C" variabletype=""&gt;一个字符串&lt;/field&gt;

                                    &lt;value name="TEXT"&gt;

                                      &lt;shadow type="text" id="cy:M1+;a\]pzNe@xbQ%~="&gt;

                                        &lt;field name="TEXT"&gt;&lt;/field&gt;

                                      &lt;/shadow&gt;

                                      &lt;block type="variables\_get" id=":\_GW7/7+@qkp5o8Qop\(D"&gt;

                                        &lt;field name="VAR" id="K:L-Tq4sa\[H;8i$GkHG\|" variabletype=""&gt;i&lt;/field&gt;

                                      &lt;/block&gt;

                                    &lt;/value&gt;

                                    &lt;next&gt;

                                      &lt;block type="text\_append" id="s\*,xO\[m\_0^V=1\#ciZURg"&gt;

                                        &lt;field name="VAR" id="tyoreQKzw\_F:U\`O4nL:C" variabletype=""&gt;一个字符串&lt;/field&gt;

                                        &lt;value name="TEXT"&gt;

                                          &lt;shadow type="text" id="IU.a\[\#3@0ouSs/{-UbO}"&gt;

                                            &lt;field name="TEXT"&gt;   &lt;/field&gt;

                                          &lt;/shadow&gt;

                                        &lt;/value&gt;

                                      &lt;/block&gt;

                                    &lt;/next&gt;

                                  &lt;/block&gt;

                                &lt;/statement&gt;

                              &lt;/block&gt;

                            &lt;/next&gt;

                          &lt;/block&gt;

                        &lt;/statement&gt;

                        &lt;next&gt;

                          &lt;block type="text\_print" id="x}U!g7=\(9d\*nPo^lYEDN"&gt;

                            &lt;value name="TEXT"&gt;

                              &lt;shadow type="text" id="PiH4GCY{;CY\`,34LEge4"&gt;

                                &lt;field name="TEXT"&gt;abc&lt;/field&gt;

                              &lt;/shadow&gt;

                              &lt;block type="variables\_get" id="\#5Pxv5cPxPx@;N\]bm\#L/"&gt;

                                &lt;field name="VAR" id="tyoreQKzw\_F:U\`O4nL:C" variabletype=""&gt;一个字符串&lt;/field&gt;

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



