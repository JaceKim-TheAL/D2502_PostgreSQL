# 오픈 소스 객체-관계형 데이터베이스 관리 시스템(ORDBMS)
---
### PostgreSQL 설치방법
방법1. Window 설치파일 실행
> - Download : <a href="">PostgreSQL 공식 웹사이트 <img src="https://www.postgresql.org/media/img/about/press/elephant.png" alt="PostgreSQL Elephant Logo" width=20></a>
> - <a href="https://www.postgresql.org/download/windows/">Downloads <img src="https://www.postgresql.org/media/img/windows.svg" alt="Windows Logo" width=20></a> 에서 `Download the installer` 클릭
> - 최신버전의 Windows x86-64 를 다운로드 후 설치 <br/> 
> ```postgresql-17.4-1-windows-x64.exe```

방법2. Scoop으로 Powershell에서 설치
> - 접속 : <a href="https://scoop.sh/">Scoop, A command-line installer for Windows</a>
> - 설치 : PowerShell terminal 에서 실행
> 
<pre style="color: rgb(57, 58, 52); font-family: Consolas, &quot;Bitstream Vera Sans Mono&quot;, &quot;Courier New&quot;, Courier, monospace; direction: ltr; text-align: left; white-space: pre; word-spacing: normal; word-break: normal; font-size: 0.9em; line-height: 1.4; tab-size: 4; hyphens: none; padding: 1em; margin: 0px; overflow: auto; border: 1px solid rgb(221, 221, 221); background-color: white;"><code style="line-height: 1.4; font-size: 0.9em; margin: 0px; white-space: pre;"><span class="token" style="color: rgb(154, 5, 15); font-weight: bold;">Set-ExecutionPolicy</span><span> </span><span class="token" style="color: rgb(57, 58, 52);">-</span><span>ExecutionPolicy RemoteSigned </span><span class="token" style="color: rgb(57, 58, 52);">-</span><span>Scope CurrentUser
</span><span></span><span class="token" style="color: rgb(154, 5, 15); font-weight: bold;">Invoke-RestMethod</span><span> </span><span class="token" style="color: rgb(57, 58, 52);">-</span><span>Uri https:</span><span class="token" style="color: rgb(57, 58, 52);">/</span><span class="token" style="color: rgb(57, 58, 52);">/</span><span>get</span><span class="token" style="color: rgb(57, 58, 52);">.</span><span>scoop</span><span class="token" style="color: rgb(57, 58, 52);">.</span><span>sh </span><span class="token" style="color: rgb(57, 58, 52);">|</span><span> </span><span class="token" style="color: rgb(154, 5, 15); font-weight: bold;">Invoke-Expression</span></code></pre>
> 
> <!--  ``` > Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser > Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression ``` > -->
> - 검색창에 `postgresql` 을 입력하고, `postgresql in main` 클릭 후 명령문을 복사
> - Terminal에서 실행 <br/>
> `PS C:> scoop install postgresql`
> - 설치 확인 <br/>
> `PS C:> scoop list postgresql`
