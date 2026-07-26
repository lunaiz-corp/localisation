# lunaiz-i18n

Lokalise에 있던 i18n 번역 사전을 [Weblate](https://weblate.org/)로 이관하기 위한 저장소입니다.
이 저장소의 파일들은 Weblate에서 프로젝트/컴포넌트 단위로 불러올 수 있도록, 프로젝트 및 도메인별로 번역 파일을 정리해 둔 것입니다.

## 디렉토리 구조

```
<프로젝트명>/<도메인명>/<로케일>/<네임스페이스>.json
```

- **프로젝트명**: 서비스 단위 (예: `payflova`)
- **도메인명**: 프로젝트 내 세부 서비스/앱 단위 (예: `payflova-checkout`)
- **로케일**: 번역 대상 언어 (예: `ko_KR`, `en_US`)
- **네임스페이스**: 화면/기능 단위로 분리된 번역 키 그룹 (예: `common`, `cart`, `error`)

## 현재 이관 현황

| 프로젝트 | 도메인 | 로케일 |
| --- | --- | --- |
| `payflova` | `payflova-checkout` | `en_GB`, `en_US`, `ja_JP`, `ko_KR`, `vi_VN`, `zh_CN`, `zh_TW` |

각 로케일 디렉토리에는 `cart.json`, `common.json`, `error.json` 네임스페이스 파일이 포함되어 있습니다.

다른 프로젝트/도메인의 사전은 이관이 진행되는 대로 이 저장소에 추가될 예정입니다.
