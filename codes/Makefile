# chap1

hello:
	cc -o hello hello.c
# -T: システムコールにかかる時間取得
chello_strace:
	strace -T -o hello.log ./hello
pyhello_strace:
	strace -o hello.py.log python3 ./hello.py

# chap2
# sysstat
# user mode: %user + %nice, kernel mode: %system
sar:
	sar -P ALL 1
loop:
	cc -o loop loop.c
# ldd: プログラムがリンクしているライブラリ
ldd:
	ldd /bin/echo

# chap3
fork:
	cc -o fork fork.c
# Linux 実行ファイルは Executable and Linkable Format(ELF) を使用する
# -h: 開始アドレスを得る、-S: ファイル内のオフセット、サイズ、開始アドレスを得る
readelf:
	readelf -h /bin/sleep && readelf -S /bin/sleep
forkandexec:
	cc -o fork-and-exec fork-and-exec.c