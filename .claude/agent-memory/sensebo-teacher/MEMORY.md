# 센세봇 학습자 메모리

마지막 업데이트: 2026-02-23

---

## 학습자 프로필

- 학습 수준: Claude Code 중급 (기본 사용법 이해 완료, 심화 기능 탐색 중)
- 선호 설명 스타일: 코드 예시 + 개념 비교
- 실습 스타일: 개념 학습 후 직접 실습, 동작 확인 후 질문

---

## 학습 완료 주제 (반복 설명 불필요)

### Claude Code 권한 및 모드 (02.md)
- Normal / Auto-Accept / Plan 3가지 모드 차이 이해 완료
- Shift+Tab 순환, `/plan` 커맨드, `--permission-mode plan` 플래그
- Ctrl+G로 계획 에디터 열기 직접 실습 완료
- Plan Mode에서 레포 분석 실습 완료

### 멀티 에이전트 / Sub-agents (03.md)
- 내장 에이전트 4종 이해: Explore(Haiku), Plan, General-purpose, Bash
- `/agents` 커맨드로 커스텀 에이전트 생성 직접 실습 완료
- 생성한 에이전트: `ml-doc-readability-reviewer` (opus, memory:project), `sensebo-teacher`
- 자동 위임 원리: `description` 필드 기반 LLM 판단
- 에이전트 별칭 패턴: `disable-model-invocation` + 커스텀 슬래시 커맨드
- 병렬 실행 vs 체이닝 패턴 이해
- 에이전트 삭제 = md 파일 삭제 이해

### Skills (04.md)
- `commands/` vs `skills/` 차이 이해: skills가 상위 집합
- skills도 슬래시 커맨드로 호출 가능 (처음엔 오해 있었음, 정정 완료)
- `disable-model-invocation` vs `user-invocable` 혼동 있었음, 정정 완료
- `commands/` -> `skills/` 마이그레이션 직접 실습 완료 (note, my-git 파일)

---

## 자주 보이는 질문 패턴

- "이것과 저것의 차이가 뭔가요?" 형태의 비교 질문을 선호함
- 직접 실습 후 "이렇게 동작하는 게 맞나요?" 확인 질문 패턴이 반복됨
- 개념 이해 후 엣지 케이스를 파고드는 경향 있음 ("그럼 이런 경우엔?")

---

## 이전에 발생한 오해 (다음 설명 시 주의)

- `skills/`를 슬래시 커맨드로 호출할 수 없다고 오해한 적 있음 -> 실제로는 가능함
- `disable-model-invocation`과 `user-invocable` 속성 혼동 -> 두 개념 명확히 분리 설명 필요

---

## 다음 세션 추천 학습 방향

- 05.md 이후 내용 (Hook, MCP 등 심화 기능)
- 멀티 에이전트 병렬 실행 패턴 실제 프로젝트에 적용해보기
- 커스텀 에이전트 description 최적화 실습
