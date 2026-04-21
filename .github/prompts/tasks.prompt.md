---
mode: agent
tools: ["codebase", "editFiles", "runCommands"]
description: Spec/Plan 기반 작업 목록을 생성합니다.
---

`specs/001-counter/spec.md`와 `specs/001-counter/plan.md`를 기준으로 `specs/001-counter/tasks.md`를 생성해 주세요.

규칙:
- 체크박스 형식 (`- [ ]`)
- 작업 ID 부여 (`T001`, `T002` ...)
- 의존성 명시
- 병렬 가능 작업 표시

작업은 실행 순서가 명확해야 하며, Spring Boot Counter 앱 구현에 직접 연결되어야 합니다.
