# web-scraping-pipeline

취업 준비하면서 매일 사람인/원티드에서 "스마트팩토리 데이터 엔지니어"를 검색하는 게 비효율적이라 직접 만든 자동 수집기

## 해결하는 문제

> 채용 사이트마다 따로 검색하고, 새 공고가 올라왔는지 매번 확인하는 시간 낭비
> 키워드 매칭으로 자동 수집 + 알림

## Stack

`Python` `requests` `BeautifulSoup` `selenium` `pandas` `schedule`

## Structure

- `scrapers/job_scraper.py` — 채용공고 크롤러
- `scrapers/energy_price.py` — OPINET 유가 크롤러
- `scrapers/realstate.py` — 국토부 실거래가 수집
- `data/` — 수집된 데이터
- `scheduler/run.py` — 자동 실행 스케줄러

## Features

| 기능 | 설명 | 상태 |
|------|------|------|
| 채용공고 크롤링 | 사람인/원티드 키워드 검색 자동화 | 예정 |
| 중복 제거 | 이미 수집한 공고 필터링 | 예정 |
| 알림 | 새 공고 발견 시 텔레그램/이메일 전송 | 예정 |
| 유가/부동산 수집 | OPINET, 국토부 API 연동 | 예정 |

## How to Run

```bash
pip install -r requirements.txt
python scrapers/job_scraper.py
```
