## 💻 MySQL 설치 가이드

> 1. 공식 홈페이지 해당 링크 접속

> https://dev.mysql.com/downloads/installer/

> 2. **다운로드** 클릭

> 3. 하단 **No thanks, just start my download** 클릭

> 4. 설치 파일 실행

> 5. **Developer Default** 클릭 후 Next

> 6. One or more product requirements have not been satisfied 가 나타나면 **Yes** 클릭

> 7. Installation 창 보이면 **Execute** 클릭

> 8. 전부 초록색 체크 표시 나타나면 Next 클릭

간혹 MySQL Shell과 Connector가 설치되지 않는 경우가 있는데, 이럴 경우에는 **현재 사용 중인 버전**을 확인해보자! 나같은 경우에는 Python Connector가 제대로 설치되지 않는 문제가 있었는데, **이전 버전으로 재설치**한 뒤

> https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170

여기서 **OS에 맞는 파일**을 다운로드 하고나니 잘 해결되었다.

> 9. Product Configuration 으로 넘어가면 Next 클릭

> 10. Type and Networking에서도 Next 클릭

> 11. Authentication Method에서 **Use Strong Password encryption for Authentication (RECOMMENDED)** 클릭 후 Next

> 12. MySQL Root Password 설정 후 Next

> 13. Windows Service에서 **Configure MySQL Server as a Windows Service** 클릭
 Windows Service Name **MySQL80**으로 설정한 뒤 **Start the MySQL Server at System Startup, Standard System Account** 클릭

 > 14. Server File Permissions에서 **Yes, grant full access to the user running th Windows Service~** 선택 후 Next 클릭

 > 15. Apply Configuration으로 넘어가면 **Execute** 클릭

 > 16. 전부 초록색 체크 표시 뜨면 Finish 클릭

 > 17. Product Configuration에서도 Next 클릭

 > 18. MySQL Router Configuration에서 **아무것도 클릭하지말고 Finish 누르기**

 > 19. 그 다음 Product Configuration에서도 Next 클릭

 > 20. Connect To Server에서 아까 설정했던 **Root Password 입력**한 뒤 Check 누르고 Next 클릭

 > 21. Status에서 초록색으로 Connection successed 출력되면 맞게 잘 수행된 것!

 > 22. Apply Configuration에서도 **Execute** 클릭

 > 23. 전부 초록색 체크 표시 뜨면 Finish 클릭

 > 24. 그 다음 Product Configuration에서도 Next 클릭

 > 25. Installation Complete 창으로 넘어가면 **체크 들어가있는거 그대로 두고 Finish 클릭**

 > 26. MySQL Shell과 MySQL Workbench, 두 개의 창이 **동시에 뜨면 설치가 정상적으로 완료**되었다는 뜻이다! 👍

 > 27. MySQL Workbench에서, Connections에 있는 Local instance 눌러서 password 입력하면 로그인 할 수 있다! 😍
