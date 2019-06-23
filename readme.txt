:1,$join
:s/\v(.{80})/\1\r/g

:set tw=76
:set fo+=t
gqq % format the current line

!fold --spaces --width=80

!fold --width=80

:setl tw=80 fo=t
1GVGgq

:set formatoptions+=w
:set tw=80
gggqG

