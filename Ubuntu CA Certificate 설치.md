# Ubuntu CA Certificate 설치

/usr/share/ca-certificates/extra 폴더를 만든다. (sudo 로)
.crt 파일을 해당 폴더로 복사한다.
(.crt 파일의 이름에 공백은 없어야 함.)

	sudo dpkg-reconfigure ca-certificates 를 실행한다.

