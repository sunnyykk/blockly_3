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

```
<xml xmlns="http://www.w3.org/1999/xhtml">
  <variables>
    <variable id="a#(mtky~+wnWkWX3B;{j" type="">n</variable>
    <variable id="v%N/?F/(pcwLd-H4]~,`" type="">和</variable>
    <variable id=",TMq3}%^r=x@5jGT,OHK" type="">积</variable>
    <variable id="-ECAVeEEGGbU.m[~z.Er" type="">x</variable>
    <variable id="u3O2!iV;g!Key-;]z::x" type="">次数</variable>
  </variables>
  <block id="UBDsPPfM[VF,7@};T/@`" type="variables_set" x="363" y="38">
    <field id="a#(mtky~+wnWkWX3B;{j" name="VAR" variableType="">n</field>
    <value name="VALUE">
      <block id="gO%NK{X8]|(^02hYOEmJ" type="math_number">
        <field name="NUM">0</field>
      </block>
    </value>
    <next>
      <block id="T3[OJ!gY2[o3iq*qXsDf" type="variables_set">
        <field id="v%N/?F/(pcwLd-H4]~,`" name="VAR" variableType="">和</field>
        <value name="VALUE">
          <block id="cpFjg0{hpS{0E.9oNl*o" type="math_number">
            <field name="NUM">0</field>
          </block>
        </value>
        <next>
          <block id="v0v@@1t-p5lfr?$t^MUT" type="variables_set">
            <field id=",TMq3}%^r=x@5jGT,OHK" name="VAR" variableType="">积</field>
            <value name="VALUE">
              <block id="jf)]_R#7GhyIuv?s}$r_" type="math_number">
                <field name="NUM">1</field>
              </block>
            </value>
            <next>
              <block id="i,ImsVjPu%^QIex3F}4q" type="variables_set">
                <field id="-ECAVeEEGGbU.m[~z.Er" name="VAR" variableType="">x</field>
                <value name="VALUE">
                  <block id="28kcF5Q5(/bdJsjRpwF+" type="math_number">
                    <field name="NUM">1</field>
                  </block>
                </value>
                <next>
                  <block id="|7,.DCJrFfMub@1RUF]#" type="controls_whileUntil">
                    <field name="MODE">WHILE</field>
                    <value name="BOOL">
                      <block id="Rv4A_ZF/aYs1]}Ui8(lb" type="logic_compare">
                        <field name="OP">LTE</field>
                        <value name="A">
                          <block id="9VDi)C9Ml`pn^IIi(,j|" type="variables_get">
                            <field id="-ECAVeEEGGbU.m[~z.Er" name="VAR" variableType="">x</field>
                          </block>
                        </value>
                        <value name="B">
                          <block id="NoPS0vUk?j|`:GjL]xI6" type="variables_get">
                            <field id="a#(mtky~+wnWkWX3B;{j" name="VAR" variableType="">n</field>
                          </block>
                        </value>
                      </block>
                    </value>
                    <statement name="DO">
                      <block id="z~}50Qw85Nb$[biy.l7G" type="variables_set">
                        <field id="u3O2!iV;g!Key-;]z::x" name="VAR" variableType="">次数</field>
                        <value name="VALUE">
                          <block id="v]qXQ_o%CT`rpqaSK$6q" type="math_number">
                            <field name="NUM">1</field>
                          </block>
                        </value>
                        <next>
                          <block id="J/LH!q)v0~zi+q[LGO#I" type="controls_whileUntil">
                            <field name="MODE">WHILE</field>
                            <value name="BOOL">
                              <block id="[7$nhtMB?Q0]E%0rr4FA" type="logic_compare">
                                <field name="OP">LTE</field>
                                <value name="A">
                                  <block id="-g4A5^Pl}[fgA?_hiL+m" type="variables_get">
                                    <field id="u3O2!iV;g!Key-;]z::x" name="VAR" variableType="">次数</field>
                                  </block>
                                </value>
                                <value name="B">
                                  <block id="Q:Zi@TQy?D@EHb|)KEFv" type="variables_get">
                                    <field id="-ECAVeEEGGbU.m[~z.Er" name="VAR" variableType="">x</field>
                                  </block>
                                </value>
                              </block>
                            </value>
                            <statement name="DO">
                              <block id="-Nr5?:TMA8B(E%,Y9QNY" type="variables_set">
                                <field id=",TMq3}%^r=x@5jGT,OHK" name="VAR" variableType="">积</field>
                                <value name="VALUE">
                                  <block id="KV*9=2+Pj)O#(1-Pl[m(" type="math_arithmetic">
                                    <field name="OP">MULTIPLY</field>
                                    <value name="A">
                                      <shadow id="4g@H|N4p#_OS/0{3X_V1" type="math_number">
                                        <field name="NUM">1</field>
                                      </shadow>
                                      <block id="R6c=#2}gkx^zwhHe*/[G" type="variables_get">
                                        <field id="u3O2!iV;g!Key-;]z::x" name="VAR" variableType="">次数</field>
                                      </block>
                                    </value>
                                    <value name="B">
                                      <shadow id="$f/z@vj(gdkPptph4NLv" type="math_number">
                                        <field name="NUM">1</field>
                                      </shadow>
                                      <block id="43^jh+dwd.jKNtPP.WNc" type="variables_get">
                                        <field id=",TMq3}%^r=x@5jGT,OHK" name="VAR" variableType="">积</field>
                                      </block>
                                    </value>
                                  </block>
                                </value>
                                <next>
                                  <block id="1ZXMQjgH$Et#.m|O2c^!" type="variables_set">
                                    <field id="u3O2!iV;g!Key-;]z::x" name="VAR" variableType="">次数</field>
                                    <value name="VALUE">
                                      <block id="00_]P^KVlq$I:%x*y2RR" type="math_arithmetic">
                                        <field name="OP">ADD</field>
                                        <value name="A">
                                          <shadow id="d[Mh7bq/Wq0}m0g5@`%j" type="math_number">
                                            <field name="NUM">1</field>
                                          </shadow>
                                          <block id="hI]y8?FGkU#rS.p5NJX9" type="variables_get">
                                            <field id="u3O2!iV;g!Key-;]z::x" name="VAR" variableType="">次数</field>
                                          </block>
                                        </value>
                                        <value name="B">
                                          <shadow id="uu[*LVSqcm4MApz[.;y7" type="math_number">
                                            <field name="NUM">1</field>
                                          </shadow>
                                        </value>
                                      </block>
                                    </value>
                                  </block>
                                </next>
                              </block>
                            </statement>
                            <next>
                              <block id="wp5QP{R?b1dZ1^]R4OJ[" type="variables_set">
                                <field id="v%N/?F/(pcwLd-H4]~,`" name="VAR" variableType="">和</field>
                                <value name="VALUE">
                                  <block id="C?v5,kojM$2j:{cL3`0u" type="math_arithmetic">
                                    <field name="OP">ADD</field>
                                    <value name="A">
                                      <shadow id="qOMR!QYPrc`k[3#8UGOB" type="math_number">
                                        <field name="NUM">1</field>
                                      </shadow>
                                      <block id="*=B*M/!~A|lf!KMb)z?_" type="variables_get">
                                        <field id=",TMq3}%^r=x@5jGT,OHK" name="VAR" variableType="">积</field>
                                      </block>
                                    </value>
                                    <value name="B">
                                      <shadow id="hZ~DZg@[lUUe?c3Qq=s=" type="math_number">
                                        <field name="NUM">1</field>
                                      </shadow>
                                      <block id="pxtH3IpHU4??*(:+O2kD" type="variables_get">
                                        <field id="v%N/?F/(pcwLd-H4]~,`" name="VAR" variableType="">和</field>
                                      </block>
                                    </value>
                                  </block>
                                </value>
                                <next>
                                  <block id="2p]UMA{2y8!.`r#!Lk81" type="variables_set">
                                    <field id=",TMq3}%^r=x@5jGT,OHK" name="VAR" variableType="">积</field>
                                    <value name="VALUE">
                                      <block id="RSEk5BKl~_WC(Q/NlR#," type="math_number">
                                        <field name="NUM">1</field>
                                      </block>
                                    </value>
                                    <next>
                                      <block id="I8(mqkNy:jV_^hMt;B.r" type="variables_set">
                                        <field id="-ECAVeEEGGbU.m[~z.Er" name="VAR" variableType="">x</field>
                                        <value name="VALUE">
                                          <block id="PIu*;Y}fn0-j:vBV/~7c" type="math_arithmetic">
                                            <field name="OP">ADD</field>
                                            <value name="A">
                                              <shadow id="1HO$~_hAnfWVJg8py(^F" type="math_number">
                                                <field name="NUM">1</field>
                                              </shadow>
                                              <block id="x6WQvQUtuAG4[K+ojd5E" type="variables_get">
                                                <field id="-ECAVeEEGGbU.m[~z.Er" name="VAR" variableType="">x</field>
                                              </block>
                                            </value>
                                            <value name="B">
                                              <shadow id="Y?[I!E=r+AI}-)p?Fg$T" type="math_number">
                                                <field name="NUM">1</field>
                                              </shadow>
                                            </value>
                                          </block>
                                        </value>
                                      </block>
                                    </next>
                                  </block>
                                </next>
                              </block>
                            </next>
                          </block>
                        </next>
                      </block>
                    </statement>
                    <next>
                      <block id="]nK69wA#P+kvw@Bcp1C{" type="text_print">
                        <value name="TEXT">
                          <shadow id="OQD=mq=oB;qMNP;tp/aG" type="text">
                            <field name="TEXT">abc</field>
                          </shadow>
                          <block id="G1yNrBrDIiM]vynEztvz" type="variables_get">
                            <field id="v%N/?F/(pcwLd-H4]~,`" name="VAR" variableType="">和</field>
                          </block>
                        </value>
                      </block>
                    </next>
                  </block>
                </next>
              </block>
            </next>
          </block>
        </next>
      </block>
    </next>
  </block>
</xml>
```

