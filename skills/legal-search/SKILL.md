---
name: Korean Legal Search
description: This skill should be used when the user asks about Korean law, legal consultation, statutes, case law, precedents, constitutional court decisions, legal interpretation, ordinances, or needs to find legal sources and URLs for Korean legal matters.
version: 0.1.0
---

# 대한민국 법률 검색 가이드

## 주요 법률 정보 소스

### 1. 국가법령정보센터 (법률/시행령/시행규칙)
- **URL**: https://www.law.go.kr
- **검색**: 법령명, 조문번호, 키워드 검색 가능
- **직접 링크 형식**: `https://www.law.go.kr/법령/[법령명]`

### 2. 대법원 종합법률정보 (판례)
- **URL**: https://glaw.scourt.go.kr
- **검색**: 사건번호, 판결요지, 키워드 검색
- **판례 형식**: 대법원 20XX.XX.XX. 선고 20XXXX 판결

### 3. 헌법재판소 (헌법재판 결정)
- **URL**: https://www.ccourt.go.kr
- **검색**: 사건번호, 결정요지 검색
- **결정 형식**: 헌재 20XX.XX.XX. 20XX헌XX

### 4. 법제처 법령해석
- **URL**: https://www.moleg.go.kr
- **검색**: 법령해석례, 행정해석 검색

### 5. 자치법규정보시스템 (조례/규칙)
- **URL**: https://www.elis.go.kr
- **검색**: 지방자치단체별 조례, 규칙 검색

### 6. 학술 자료
- **한국학술정보(KISS)**: https://kiss.kstudy.com
- **한국학술지인용색인(KCI)**: https://www.kci.go.kr
- **법학 논문 데이터베이스**: https://www.riss.kr

## 검색 전략

### 법률조항 검색
1. 관련 법령명 확인
2. 해당 조문 번호 특정
3. 국가법령정보센터에서 직접 링크 생성

### 판례 검색
1. 관련 법률 키워드로 검색
2. 대법원/고등법원/지방법원 구분
3. 최신 판례 우선 확인

### 복합 검색
1. 여러 법령이 관련된 경우 각각 검색
2. 상위법-하위법 관계 확인
3. 특별법-일반법 관계 확인

## 결과 제공 형식

검색 결과는 다음 형식으로 제공합니다:

```
## 관련 법률
- [법령명 제X조](URL) - 조문 내용 요약

## 관련 판례
- [대법원 20XX.XX.XX. 선고 20XXXX 판결](URL) - 판결 요지

## 참고 자료
- [자료명](URL) - 간략 설명
```

## 주의사항

- 법률 정보는 참고용이며, 정확한 법률 자문은 변호사 상담 권장
- 법령 개정 여부 항상 확인 필요
- 판례의 경우 사실관계 차이에 따라 적용이 달라질 수 있음
