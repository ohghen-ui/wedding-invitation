# 오건 ♥ 카리나 모바일 청첩장 — GitHub Pages

## 가장 쉬운 배포 방법 (GitHub 웹사이트에서)

1. https://github.com/new 에 접속 후 로그인합니다.
2. Repository name에 `wedding-invitation` 입력 → **Public** 선택 → Create repository.
3. 저장소의 **Add file → Upload files**에서 `index.html`, `.nojekyll`, `assets` 폴더의 `wedding-photo.png`, `thumbnail.jpg`를 올립니다. (브라우저에서는 폴더 내 파일을 함께 드래그하거나 GitHub Desktop을 사용하는 것이 편합니다.)
4. 자동 미리보기(OG URL 자동 변환)를 위해 `.github/workflows/deploy.yml` 파일을 반드시 같은 경로에 업로드해야 합니다. 웹에서 **Add file → Create new file**을 선택한 다음 파일 이름 `.github/workflows/deploy.yml`로 지정하고 이 배포본의 내용을 붙여넣어 저장해도 됩니다.
5. 저장소 **Settings → Pages → Build and deployment → Source: GitHub Actions** 선택.
6. 상단 **Actions** 탭에서 배포 작업이 초록색으로 성공했는지 확인합니다.
7. `https://내깃허브아이디.github.io/wedding-invitation/` 에서 확인하세요.

> ZIP 자체를 Github 저장소에 파일 하나로 업로드하는 것만으로는 배포되지 않습니다. 압축을 풀어 **구조대로** 올려야 합니다.

## 공유 썸네일

- 이미지: `assets/thumbnail.jpg` (1200 x 630, JPG, 실제 웨딩사진 기반)
- 배포 과정에서 `og:image`를 실제 GitHub Pages 절대주소로 자동 변환합니다.
- 카카오톡에 실제 사이트 URL을 공유하면 제목·설명·사진이 표시되도록 준비되어 있습니다. 카카오톡 캐시나 접근 상태 때문에 반영에 시간이 걸릴 수 있습니다.
- 이전 썸네일이 보이면 카카오 공유 디버거(https://developers.kakao.com/tool/clear/og)에서 사이트 URL의 캐시를 초기화하세요.

## 개인정보 주의

- 이 정적 사이트는 공개 저장소 및 공개 웹주소에 계좌번호와 웨딩 사진이 표시됩니다.
- 계좌번호가 노출되어도 되는지 확인 후 배포하세요.
- 기존 thegoodday.kr 주소의 원본을 변경하는 것이 아니라 **새로운 GitHub Pages 링크**입니다.

## 로컬 실행

index.html을 더블클릭하면 사진, 계좌번호, 지도, 복사 버튼을 확인할 수 있습니다. 공유 미리보기는 GitHub Pages에 배포한 후 URL을 공유해야 동작합니다.
