# Taxi DJ v4 - 원터치 유튜브 DJ PWA

택시 운행 중 2터치로 음악 재생하는 iOS PWA

## 기능
- **오프라인 보관함**: IndexedDB 영구 저장, 10시간 재즈 mp3 무광고 0GB 재생
- **유튜브 오프라인 보관함 바로 열기**: `m.youtube.com/feed/downloads` 링크로 유튜브 앱 점프
- **YT뮤직 DJ 탭**: `music.youtube.com/search?q=` 로 검색, 데이터 0.7GB/10h
- **롱믹스 10시간 탭**: 10시간 무광고 영상 검색
- 프리셋 편집, 테더링 30GB/80GB 표시, 하단 플레이어는 오프라인 탭에서만 표시

## 아이폰 아이콘
- `icons/apple-touch-icon.png` (180x180) - 홈화면 아이콘
- `icons/icon-192.png`, `icon-512.png` - PWA manifest
- `icon-1024.png` - App Store용 (필요시)

## 깃허브 Pages 발행
1. 깃허브에 `taxi-dj` 레포 생성
2. 이 폴더 전체 업로드 (index.html, manifest.json, sw.js, icons/)
3. Settings > Pages > Source: main branch / root 선택
4. 배포 URL: `https://USERNAME.github.io/taxi-dj/`
5. iPhone Safari에서 열고 공유 > 홈 화면에 추가

## 로컬 테스트
```bash
npx serve .
```

## 데이터 절약
- 오프라인: 0GB
- YT뮤직: 10시간 0.7GB
- 유튜브 영상: 10시간 12GB

프리미엄 로그인 시 유튜브 앱으로 자동 전환되어 무광고 재생됨.
