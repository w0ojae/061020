# Lazy Day · GitHub Pages 업로드용 전체 파일

최신 작업 v35 · 2026-10-20 · 원본 커밋 6d86c9a97ecf9869365694c2d3d3f4225c3a1f53

이 ZIP에는 건물 모델, Three.js, 창문 빗방울 텍스처와 물리, 실내·정원 이동, 의자 상호작용, 셰이더, 새, 시작 화면, 5분 하루, 느린 UI 색상 전환이 포함됩니다. 실행 파일 58개를 모두 포함한 독립적인 전체 배포본입니다.

## GitHub에 올리는 방법

1. ZIP을 압축 해제합니다.
2. 저장소의 Add file 메뉴에서 Upload files를 선택합니다.
3. 압축을 푼 폴더 안의 파일과 하위 폴더를 전부 업로드합니다. 저장소 최상위에서 index.html과 assets, vendor, rain, weather, style 폴더가 바로 보여야 합니다.
4. Commit changes로 저장합니다. 기존 파일이 있으면 이번 파일로 교체합니다.
5. 저장소 Settings의 Pages에서 Source를 Deploy from a branch로 설정합니다.
6. Branch는 업로드한 브랜치(main 등), 폴더는 /(root)로 선택하고 Save를 누릅니다.
7. 배포가 완료되면 Pages 설정에 표시되는 주소를 엽니다. 예를 들어 w0ojae 계정의 261013 저장소라면 https://w0ojae.github.io/261013/ 입니다.

ZIP 파일 자체가 아니라 압축을 푼 내용물을 올려야 합니다. 상위 폴더까지 넣어 index.html이 한 단계 안쪽에 들어가지 않도록 최상위 배치를 확인하세요. 업로드 파일은 100개 이하이고 가장 큰 파일도 25MiB 이하입니다.

## 업로드 후 확인

- 저장소 최상위에 index.html, main-garden.js, style.css가 있습니다.
- assets/building2.glb, vendor/three.module.js, vendor/three.core.js가 있습니다.
- rain/assets/drop-alpha.png와 drop-color.png가 있습니다.
- .nojekyll과 _config.yml도 함께 올립니다. vendor 폴더가 게시 중 생략되지 않도록 준비했습니다.
- Pages에 Published 또는 배포 성공이 표시된 뒤 주소를 엽니다. 기존 탭이 있으면 새로고침합니다.

별도 npm 설치·빌드·API 키가 필요하지 않습니다. 파일을 더블클릭하는 대신 GitHub Pages의 HTTPS 주소에서 실행하세요. Google Fonts는 기존과 같이 외부에서 불러오며 연결되지 않으면 시스템 글꼴을 사용합니다.

## 백업과 출처

원래 개발 폴더 구조, 검사 스크립트, package.json은 별도 Lazy-Day-Source-Backup-v35-2026-10-20.zip에 보관했습니다. 이 업로드용 ZIP은 웹 실행에 필요한 원본 dist 파일을 모두 최상위로 옮긴 배포본입니다. Git 이력과 Sites 배포 관리용 .openai 파일은 업로드본에 필요하지 않습니다.

vendor/THREE-LICENSE.txt와 rain/THIRD_PARTY_NOTICES.md를 유지하세요. 건물 GLB와 모든 기존 실행 파일의 내용은 그대로 보존했으며 backup-manifest.json에 파일별 SHA-256을 기록했습니다.

공식 설정 안내: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
공식 업로드 안내: https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
