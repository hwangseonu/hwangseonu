```sh
$ whoami --json
```

```json
{
  "name": "황선우",
  "handle": "hwangseonu",
  "email": "contact@kinoshita.dev",
  "languages": {
    "ko": "한국어",
    "ja": "日本語",
    "en": "beginner"
  },
  "focus": [
    "AI",
    "Full Stack",
    "Product Engineering"
  ]
}
```

# Education

- 대덕소프트웨어마이스터고등학교 정보보안과 중퇴
- Best of the Best (차세대 보안 리더 양성 프로그램) 8기 보안제품개발트랙 수료
- 소프트웨어마에스트로 11기 수료

# Projects

## [iloa.gg](https://iloa.gg)

리빌딩 프로젝트에 백엔드 보조 개발자로 참여했습니다. 이후 게임 패치에 따른 백엔드 유지보수를 담당하고, 직접 게임을 플레이하며 느낀 필요를 바탕으로 숙제관리 기능을 개발했습니다.

- **수집품 랭킹 API 개발 및 집계 구조 개선**: 원정대와 수집품 데이터를 JOIN하고 SUM으로 점수를 계산하던 API에 비정규화를 적용했습니다. 이후에도 성능 문제가 남아, 실시간 갱신이 필수적이지 않다고 판단하고 랭킹 조회 전용 테이블을 분리해 2시간마다 전체 데이터를 배치로 집계하도록 전환했습니다.
- **숙제관리의 캐릭터 레벨 갱신 시간 단축**: 대상 외의 원정대 내 캐릭터까지 갱신하고, 갱신 작업을 순차 처리하는 문제를 발견했습니다. 갱신 범위를 대상 캐릭터로 한정하고 병렬 처리하도록 변경해 소요 시간을 단축했습니다.
- **캐릭터 통계 API 개발 및 DuckDB 도입 제안**: 통계 API를 개발하며 기존 쿼리 방식의 한계를 느껴 DuckDB 도입을 제안했습니다.
- **에이전트 기반 개발을 위한 문서화**: `AGENTS.md`에 프로젝트 구성, 패키지 계층, 코딩 규칙, 모노레포 규칙을 정리했습니다.

## [gin-restful](https://github.com/hwangseonu/gin-restful)

Flask-RESTful에서 착안한 Go 라이브러리로, Gin에서 리소스 단위로 REST API를 구현할 수 있도록 개발했습니다. 리소스가 구현한 HTTP 메서드에 해당하는 라우트를 자동으로 등록합니다.

- **메서드별 인터페이스 분리**: `Lister`, `Getter`, `Poster`, `Putter`, `Patcher`, `Deleter`를 독립된 인터페이스로 제공해 필요한 메서드만 구현할 수 있도록 했습니다.
- **요청 바인딩 및 에러 응답 처리**: 제네릭 기반의 `Bind[T]`, `MustBind[T]`와 `HTTPError`, `Abort()`를 제공해 요청 데이터 바인딩과 에러 응답 처리를 지원합니다.
- **기존 Gin 코드와의 호환**: `gin.IRouter`를 받아 라우트 그룹과 미들웨어를 활용하고, 일반 Gin 핸들러와 리소스 기반 API를 함께 사용할 수 있도록 했습니다.

# Skills

## Languages

`Go` `Kotlin` `Java` `TypeScript` `JavaScript` `Python` `PHP` `Swift`

## Backend

`Gin` `Echo` `gRPC` `fasthttp` `Spring` `Ktor` `NestJS` `Express` `Koa` `Flask` `Django` `Laravel`

## Frontend

`React` `Svelte` `Vue` `jQuery`

## Mobile

`Jetpack Compose` `Kotlin` `SwiftUI` `React Native`

## Databases & Caching

`MySQL` `MariaDB` `PostgreSQL` `MongoDB` `Redis` `DuckDB`

## AI Tools & Platforms

`Claude` `Codex` `OpenRouter` `Orca` `T3 Code`

## Tools & Infrastructure

`Git` `Docker`
