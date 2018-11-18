# buildlib-openssl

///////////////////////////////////////////////////////////////////
openssl
///////////////////////////////////////////////////////////////////
编译环境:win\mingw64\gcc8.1 git-bash，git目录下
env:win\mingw64\gcc8.1 git-bash

准备工作:需要下载strawberry-perl并找到\perl\lib\的pod库放到git下自带perl的库中
before compile:download strawberry-perl and replace pod library from c:\perl\lib\ to git\perl\\

编译脚本:
usage:
./config -fPIC no-shared
make install -j8

-fPIC：指示生成位置无关的代码，这个选项是在把openssl生成的静态库链接到动态库的时候提示错误添加的
no-shared：指示生成静态库
///--openssldir
此目录下取C:\Program Files\Git\usr\local\
in this folder:C:\Program Files\Git\usr\local\
