常用抓取命令
adb shell rm /sdcard/capture.pcap
adb shell /data/local/tcpdump -i any -p -s 0 -w /sdcard/capture.pcap

adb pull /sdcard/capture.pcap capture.pcap

tcpdump 参数说明:
# "-i any": listen on any network interface
　　# "-p": disable promiscuous mode (doesn't work anyway)
　　# "-s 0": capture the entire packet
　　# "-w": write packets to a file (rather than printing to stdout)
