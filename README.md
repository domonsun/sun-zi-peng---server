# sun-zi-peng---server
#coding: utf-8
import socket
s = socket.socket(socket.AF_INET,socket.SOCK_DGRAM)
s.bind((''0.0.0.0,8888))
print('wait for connecting...')

while True:
    conn,addr = s.recvfrom(1024)
    str1 = conn.secode('utf-8')
    print('I received a string is: ',str1)
    str2 = str1.upper()
    s.sendto(srt2.encode('utf-8'),addr)
    if str1 --'.':
        breck
s.cloce()
