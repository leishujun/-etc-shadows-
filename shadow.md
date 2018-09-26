# **/etc/shadow文件的格式**
```
wang:$6$bxKPUJM6$7Eaxgvsly3Vs2FA7vT.BrG5in9kfZ8MyaBvy4wiQ3TR/lgl4oLCYDMenMb1NMe7Ddashzu3Hq733NNT/AFc990:17800:0:99999:7:1:17900:
```

wang：用户

$6$bxKPUJM6$7Eaxgvsly3Vs2FA7vT.BrG5in9kfZ8MyaBvy4wiQ3TR/lgl4oLCYDMenMb1NMe7Ddashzu3Hq733NNT/AFc990：加密算法和密码

17800：1970年1月1日据今有17800个小时，echo   `date +%s`/3600/24   |  bc  得到的数字大概是在17800左右

0：最短密码有效期，就是说时间段内普通用户是否能修改密码，如果上面上是3的话三天内是不能修改密码的，是0的话就是说可以随意修改密码

99999：密码最长有效期，从17800那一天开始算起，往后推99999密码才会到期

7：到期前7天提醒用户修改密码

1：宽限期，过期后再给一天时间，若是这一天内还是未修改密码，就锁定账户

17900：账户到距离1970年17900天后就到期不能使用了
