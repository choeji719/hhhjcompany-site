# 호형호제 앱 웹사이트

탭메모와 출시 준비 중인 살림곁을 소개하는 정적 웹사이트입니다. `dist/`가 배포 폴더입니다.

## Render 배포

이 폴더를 별도 Git 저장소의 루트로 올리면 `render.yaml`을 사용해 정적 사이트를 만들 수 있습니다. Render 대시보드에서 직접 설정할 경우 서비스 유형은 **Static Site**, 빌드 명령은 `echo "Static site ready"`, 배포 폴더는 `dist`입니다.

## 도메인과 AppLovin

회사 사이트는 Render의 `https://hhhjcompany.com/`에서 운영합니다. 앱별 소개 페이지는 GitHub Pages에서 `tapmemo.hhhjcompany.com`, `salimgyeot.hhhjcompany.com`으로 운영합니다. 두 앱 주소의 DNS CNAME 대상은 `choeji719.github.io`입니다. `moa.hhhjcompany.com`은 별도 서비스이므로 해당 CNAME 레코드를 유지합니다.

앱별 저장소: [탭메모](https://github.com/choeji719/hhhjcompany-tapmemo), [살림곁](https://github.com/choeji719/hhhjcompany-salimgyeot). GitHub Pages의 새 도메인 인증서 발급이 끝나면 각 저장소의 Settings → Pages에서 **Enforce HTTPS**를 켭니다.

AppLovin MAX 회원가입 시 개발자 도메인은 `hhhjcompany.com`으로 입력합니다. 플레이스토어의 탭메모 개발자 웹사이트도 같은 도메인으로 설정해야 합니다. MAX가 제공하는 광고 판매자 항목을 받은 뒤에만 `dist/app-ads.txt`를 만들고, 배포 후 `https://hhhjcompany.com/app-ads.txt`에서 정확한 내용이 보이는지 확인합니다.

탭메모 플레이스토어 주소: <https://play.google.com/store/apps/details?id=com.choeji.tapmemo>
