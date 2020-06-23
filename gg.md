Generate Dump Output:
From Linux Terminal enter:
$] sdb root on
$] sdb shell
From Device (Tizen) Terminal:
sh-3.2] dumpsys batterstats > /tmp/battery_dump.txt
sh-3.2] exit
From Linux Terminal enter:
$] sdb pull /tmp/battery_dump.txt .
This “battery_dump.txt” file is the final output.
