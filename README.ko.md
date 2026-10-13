<div align="center">

![Web AR Playground](docs/readme-banner.svg)

# Web AR Playground

마커 위에 애니메이션 3D 모델을 띄우는 웹 AR 실험입니다.

[English](README.md) · **한국어**

![project: experiment](https://img.shields.io/badge/project-experiment-22d3ee?style=flat-square) ![stack: A-Frame / AR.js](https://img.shields.io/badge/stack-A--Frame%20%2F%20AR.js-22d3ee?style=flat-square)

[Repository](https://github.com/wilgon456/WebAR_test)

</div>

---

## 소개

A-Frame, AR.js, 제스처 처리 스크립트를 조합해 사용자 지정 마커 위에 `assets/asset.glb`를 표시합니다. 웹캠 입력과 반복 애니메이션을 사용합니다.

## 로컬 실행

```bash
git clone https://github.com/wilgon456/WebAR_test.git
cd WebAR_test
python3 -m http.server 8000
```

**http://localhost:8000**을 열고 카메라 권한을 허용합니다. 휴대전화나 다른 컴퓨터로 접속하려면 **HTTPS**로 제공하세요. 일반 LAN HTTP 주소에서는 카메라 권한을 받지 못할 수 있습니다.

`assets/marker.patt`와 일치하는 마커 이미지를 카메라에 보여 줍니다. 이 파일은 AR 패턴 정의이며 인쇄용 이미지가 아닙니다. 원본 마커 그림은 별도로 포함되어 있지 않습니다.

## 파일

| 파일 | 용도 |
| --- | --- |
| `index.html` | AR 장면·마커 설정·제스처 연결 |
| `assets/asset.glb` | 애니메이션 3D 모델 |
| `assets/marker.patt` | 사용자 지정 마커 패턴 |

## 실험 시 참고

외부 CDN과 upstream 브랜치에서 라이브러리를 불러오므로 서비스 상태와 브라우저 호환성에 따라 결과가 달라질 수 있습니다. 마커 일치 여부·조명·카메라 지원도 중요합니다. 여러 기기에서 검증된 AR 제품이 아닌 작은 실험 프로젝트입니다.
