# Law Plugin (법률 자문 플러그인)

대한민국 법률조항과 판례를 다방면에서 검색하여 URL로 제공하는 Claude Code 플러그인입니다.

## 기능

### 🔍 다방면 병렬 검색

6개의 전문화된 에이전트가 **동시에 병렬로** 실행되어 다양한 소스에서 법률 정보를 검색합니다:

| 에이전트 | 검색 대상 | 주요 소스 |
|---------|----------|----------|
| `statute-search-agent` | 법률조항 | 국가법령정보센터 (law.go.kr) |
| `case-law-agent` | 판례 | 대법원 종합법률정보 (glaw.scourt.go.kr) |
| `constitutional-agent` | 헌법재판 | 헌법재판소 (ccourt.go.kr) |
| `legal-interpretation-agent` | 법령해석 | 법제처 (moleg.go.kr) |
| `academic-legal-agent` | 학술자료 | KCI, RISS, 법학논문 |
| `local-ordinance-agent` | 조례 | 자치법규정보시스템 (elis.go.kr) |

### 📋 명령어

- `/law-search` - 법률 자문 요청 시 6개 에이전트 병렬 실행

### 📚 스킬

- **Korean Legal Search** - 대한민국 법률 검색 가이드 및 URL 형식 안내

## 설치

```bash
claude --plugin-dir /Users/choiwon/business/common/plugins/law-plugin
```

## 사용법

1. Claude Code 실행 시 플러그인 자동 로드
2. 법률 관련 질문 입력 또는 `/law-search` 명령어 사용
3. 6개 에이전트가 병렬로 검색 수행
4. 각 소스별 URL과 함께 결과 제공

### 예시

```
사용자: 근로기준법상 연차휴가에 대해 알려줘

결과:
- 관련 법률조항 (근로기준법 제60조) + URL
- 관련 판례 (대법원 판결) + URL
- 법령해석례 + URL
- 관련 학술논문 + URL
```

## 검색 소스

### 공식 법률 정보
- 국가법령정보센터: https://www.law.go.kr
- 대법원 종합법률정보: https://glaw.scourt.go.kr
- 헌법재판소: https://www.ccourt.go.kr
- 법제처: https://www.moleg.go.kr

### 학술 정보
- 한국학술지인용색인(KCI): https://www.kci.go.kr
- 학술연구정보서비스(RISS): https://www.riss.kr

### 지방자치법규
- 자치법규정보시스템: https://www.elis.go.kr

## 주의사항

⚠️ **면책 조항**
- 이 플러그인이 제공하는 법률 정보는 참고용입니다
- 정확한 법률 자문은 반드시 변호사에게 문의하세요
- 법령 개정 여부를 항상 확인하세요
- 판례의 경우 사실관계에 따라 적용이 달라질 수 있습니다

## 라이선스

MIT License

## 작성자

choiwon
