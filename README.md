# 수입축산물 검역중량 대시보드

공공데이터포털 API 기반, 매일 자동 갱신되는 수입축산물 검역중량 현황 대시보드.

- 사이트: https://jeruhe2-sketch.github.io/Import-Quarantine-Dashboard/
- 데이터 갱신: `scripts/update_data.py` (GitHub Actions로 매일 자동 실행)
- 원래 `jeruhe2-sketch/Livestock-Revolution` (창고 재고 대시보드)와 한 저장소에
  같이 있었는데, 서로 무관한 프로젝트라 분리함.

## Secrets 설정 필요
GitHub Actions가 공공데이터포털 API를 호출하려면 저장소 Settings → Secrets and
variables → Actions 에 `OPEN_API_KEY`를 등록해야 합니다 (기존 Livestock-Revolution
저장소에 등록되어 있던 것과 동일한 값).
