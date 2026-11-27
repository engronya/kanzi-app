APK 만들기 (GitHub가 대신 빌드해 줍니다) - PC에서 진행하세요

1) https://github.com 로그인 > 오른쪽 위 + > New repository
   이름: kanji-app, Public 선택 > Create repository
2) 만들어진 저장소 화면에서 "uploading an existing file" 클릭
3) 이 zip을 푼 폴더 안의 항목 4개를 끌어다 놓기:  www 폴더, package.json, capacitor.config.json, .gitignore
   > 아래 Commit changes 클릭
4) 같은 화면에서 Add file > Create new file
   - 파일 이름 칸에  .github/workflows/build.yml  입력 (슬래시를 치면 폴더가 만들어집니다)
   - 내용 칸에 이 zip의 .github/workflows/build.yml 내용을 복사해 붙여넣기 > Commit changes
5) 저장소 위쪽 Actions 탭 > "Build APK" 가 자동으로 실행됩니다 (약 5~8분).
   초록 체크가 뜨면 그 실행을 클릭 > 아래 Artifacts 의 kanji-app-apk 다운로드
6) 받은 zip을 풀면 app-debug.apk 가 있습니다. 스마트폰으로 옮겨 설치
   (설정에서 '출처를 알 수 없는 앱 설치' 허용 필요)

빨간 X가 뜨면 실행 화면의 오류 내용을 알려주세요.
