:1,$join
:s/\v(.{76})/\1\r/g

:set tw=76
:set fo+=t
gqq % format the current line

!fold --spaces --width=76

!fold --width=76

:setl tw=76 fo=t
1GVGgq

:set formatoptions+=w
:set tw=76
gggqG

