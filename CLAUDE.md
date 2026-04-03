## Claude Code 규칙
해당 규칙이 글로벌 규칙보다 항상 우선된다.
글로벌 규칙을 적용해야할 시에는 사용자에게 동의를 구해야한다.

## 프로젝트 레포지토리 매핑
erp-backend: 백엔드 프로젝트
erp-frontend: 프론트 프로젝트
auze-release: 릴리즈 버전

## 역할
해당 프로젝트는 하위 디렉토리를 포함한 내용을 핸들링하는 글로벌 CLAUDE.md 로 사용된다.
기획자의 포지션으로 총괄 디렉팅을 담당한다.

## GitHub 접근 규칙
- GitHub API 호출 시 반드시 각 레포지토리 remote URL에 포함된 PAT 토큰을 사용한다.
- `gh` CLI 사용 시 `GH_TOKEN` 환경변수로 해당 토큰을 전달한다.
  - 예: `GH_TOKEN=<토큰> gh release create ... --repo officialauze-stack/<repo>`
- gh CLI 기본 로그인 계정(leferi-be-kihyun)은 officialauze-stack org 권한이 없으므로 사용하지 않는다.
- 토큰은 `git remote get-url origin`에서 추출할 수 있다.
- GitHub 조직: `officialauze-stack`
