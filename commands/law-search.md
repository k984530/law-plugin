---
name: law-search
description: 대한민국 법률조항과 판례를 다방면에서 병렬 검색하여 자문 제공
---

# 법률 검색 명령어

사용자가 법률 자문을 요청하면, 다음 에이전트들을 **병렬로** 실행하여 다방면에서 법률 정보를 수집합니다.

## 실행 방법

사용자의 법률 질문에 대해 아래 6개 에이전트를 **동시에 병렬로** Task 도구를 사용하여 실행하세요:

1. **statute-search-agent**: 법률조항 검색 (국가법령정보센터)
2. **case-law-agent**: 판례 검색 (대법원 종합법률정보)
3. **constitutional-agent**: 헌법재판소 결정 검색
4. **legal-interpretation-agent**: 법령해석 및 행정해석 검색
5. **academic-legal-agent**: 법학 논문 및 학술자료 검색
6. **local-ordinance-agent**: 지방자치단체 조례 검색

## 병렬 실행 예시

```
Task 도구를 사용하여 6개 에이전트를 하나의 메시지에서 동시에 호출합니다.
각 에이전트는 독립적으로 검색을 수행하고 결과를 반환합니다.
```

## 산출물

각 에이전트는 `law-search-results/` 디렉토리에 마크다운 파일로 결과를 저장합니다:

| 에이전트 | 산출물 파일 |
|---------|------------|
| statute-search-agent | `law-search-results/statutes.md` |
| case-law-agent | `law-search-results/case-law.md` |
| constitutional-agent | `law-search-results/constitutional.md` |
| legal-interpretation-agent | `law-search-results/interpretation.md` |
| academic-legal-agent | `law-search-results/academic.md` |
| local-ordinance-agent | `law-search-results/ordinances.md` |

## 결과 정리

모든 에이전트 실행 완료 후, `law-search-results/` 디렉토리의 파일들을 종합하여 사용자에게 안내합니다:

1. **관련 법률조항**: `statutes.md` 참조
2. **관련 판례**: `case-law.md` 참조
3. **헌법재판소 결정**: `constitutional.md` 참조
4. **법령해석**: `interpretation.md` 참조
5. **학술자료**: `academic.md` 참조
6. **관련 조례**: `ordinances.md` 참조

## 중요 사항

- 모든 검색 결과는 반드시 **출처 URL**을 포함해야 합니다
- 법률 정보는 참고용이며, 정확한 법률 자문은 변호사에게 문의하도록 안내하세요
- 최신 법령 정보 확인을 권장하세요
