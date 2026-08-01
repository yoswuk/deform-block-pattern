# 디폼블럭 도안 만들기

이미지를 실제 판매되는 디폼블럭 색상에 맞춘 격자 도안으로 변환하는 웹앱입니다.

**[웹에서 바로 사용하기](https://yoswuk.github.io/deform-block-pattern/)**

## 주요 기능

- JPG, PNG, WEBP 이미지 업로드 및 브라우저 내 로컬 처리
- 가로·세로 8–160칸 자유 해상도 설정
- 최대 사용 색상 4–32색 조절
- 국내 8mm 디폼블럭 판매 색상 기반 팔레트
- 8mm 블록 기준 예상 완성 크기 계산
- 색상별 필요 블록 수량 집계
- 흰색 배경 비우기, 이미지 채우기/맞추기
- 도안 확대·축소, PNG 저장, 인쇄
- 모바일 반응형 화면

> 화면에 표시되는 RGB 값은 판매 색상표를 바탕으로 한 근사값입니다. 실제 블록의 색상은 제조 시기, 조명 및 디스플레이에 따라 다를 수 있습니다.

## 로컬 실행

Node.js 22.13 이상이 필요합니다.

```bash
npm install
npm run dev
```

프로덕션 빌드 검증:

```bash
npm run build
```

## 개인정보

업로드한 이미지는 서버로 전송하지 않습니다. 이미지 변환, 색상 양자화 및 도안 생성은 모두 사용자의 브라우저에서 수행됩니다.

## 기술 구성

- React 19
- Next.js / Vinext
- TypeScript
- HTML Canvas

## 색상표 참고

- [디폼/88 블럭 색상별 판매 목록](https://www.allcrart.com/m/product.html?branduid=71860)

## License

MIT
