# resource
Good resources for multiple languages, programming methodologies, and etc.

## php
MVC모델을 적용한 블로그(게시판) 만들기 - 0.개념 정리 및 준비하기
  https://freehoon.tistory.com/68?category=708152
MVC모델을 적용한 블로그(게시판) 만들기 - 1. Front Controller(요구사항 받아들이기)
  https://freehoon.tistory.com/69?category=708152
MVC모델을 적용한 블로그(게시판) 만들기 - 2. Controller 
  https://freehoon.tistory.com/70?category=708152
MVC모델을 적용한 블로그(게시판) 만들기 - 3. Model (DB 처리 하기) 
  https://freehoon.tistory.com/71?category=708152

MVC Project - Assignment Handler (YOUTUBE)
Create a PHP Application | PHP MVC Project Tutorial
https://www.youtube.com/watch?v=Rkg731t47dc

MVC - Model, View, Controller의 올바른 역할 분담
https://stackoverflow.com/questions/18949844/how-to-correctly-pass-data-from-controller-to-view

## css
Flexbox를 이용해서 footer를 항상 아래에 위치시키는 방법
https://dev.to/akshay_rajput/keep-footer-at-bottom-of-page-using-flexbox-4a6f

## tcp/ip
패킷이 네트워크 상에서 전달되는 방법 - datalink(L2), ip(L3) 헤더를 중심으로
:: MAC/IP Destination & Source Address
https://www.practicalnetworking.net/series/packet-traveling/packet-traveling/


# Things to learn to be a hacker
- Kali Linux
- Linux Shell Scripting
- TCP/IP
- Python

# After installing Kali linux
1. 비밀번호 변경
 - kali/kali --> ***********
2. 한글 패치
 - $ sudo apt update
 - $ sudo apt install -y fcitx-lib*
 - $ sudo apt install -y fcitx-hangul
 - $ sudo apt install -y fonts-nanum*
 - $ sudo reboot
 - input, fcitx 설정

install_hangul.sh
=================================================
#!/bin/bash
apt update
apt install -y fcitx-lib*
apt install -y fcitx-hangul
apt install -y fonts-nanum*
echo "Installation completed."
while :; do
        echo -en "Need to reboot the machine. Reboot now? [Y/n] "
        read REBOOT
        case "$REBOOT" in
                "Y"|"y")
                        echo "Rebooting machine in 3 seconds..."
                        sleep 3s
                        reboot
                        ;;
                "N"|"n")
                        echo "Reboot aborted."
                        echo "Bye..."
                        break
                        ;;
                *)
                        echo "Invalid input: Try again..."
                        ;;
        esac
done
=================================================
