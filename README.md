# web-scraping-pipeline

웹 크롤링 기반 데이터 자동 수집 파이프라인

## Stack

`Python` `requests` `BeautifulSoup` `selenium` `pandas` `schedule`

## Structure

```
web-scraping-pipeline/
├── scrapers/             # 사이트별 크롤러
│   ├── news_scraper.py
│   └── job_scraper.py
├── data/                 # 수집된 데이터
├── scheduler/            # 자동 실행 스케줄러
└── notebooks/            # 수집 데이터 분석
```

## Projects

| # | 주제 | 타겟 사이트 | 핵심 스킬 | 상태 |
|---|------|----------|----------|------|
| 01 | 뉴스 크롤러 | 네이버 뉴스 | requests, BS4, 파싱 | 예정 |
| 02 | 채용공고 수집기 | 사람인/원티드 | selenium, 동적 크롤링 | 예정 |
| 03 | 자동 수집 파이프라인 | 위 타겟 통합 | schedule, CSV 적재, 중복제거 | 예정 |

## How to Run

```bash
pip install requests beautifulsoup4 selenium pandas schedule
python scrapers/news_scraper.py
```
