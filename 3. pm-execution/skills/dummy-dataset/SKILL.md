---
name: dummy-dataset
description: "기능 테스트를 위해 사용자 정의 열, 제약 조건 및 출력 형식(CSV, JSON, SQL, Python 스크립트)을 포함하는 현실적인 더미 데이터셋을 생성합니다. 테스트 데이터 생성, 샘플 데이터셋 제작 또는 개발을 위한 모킹(mock) 데이터 구축 시 사용하세요. 트리거: 더미 데이터, 테스트 데이터, 모의 데이터셋, 샘플 데이터, 데이터 생성."
---

# 더미 데이터셋 생성

테스트를 위해 사용자 정의 열, 제약 조건 및 출력 형식(CSV, JSON, SQL, Python 스크립트)을 갖춘 현실적인 더미 데이터셋을 생성합니다. 즉시 사용할 수 있도록 실행 가능한 스크립트나 직접적인 데이터 파일을 만듭니다.

**언제 사용하나:** 테스트 데이터 작성, 샘플 데이터셋 생성, 개발을 위한 현실적인 모의 데이터 구축 또는 테스트 환경에 데이터 채우기.

**인수:**

- `$PRODUCT`: 제품 또는 시스템 이름
- `$DATASET_TYPE`: 데이터 유형 (예: 고객 피드백, 거래 내역, 사용자 프로필)
- `$ROWS`: 생성할 행 수 (기본값: 100)
- `$COLUMNS`: 포함할 특정 열 또는 필드
- `$FORMAT`: 출력 형식 (CSV, JSON, SQL, Python 스크립트)
- `$CONSTRAINTS`: 추가 제약 조건 또는 비즈니스 규칙

## 단계별 프로세스

1. **데이터셋 유형 식별** - 데이터 도메인 이해
2. **열 사양 정의** - 이름, 데이터 유형 및 값 범위
3. **행 수 결정** - 필요한 샘플 레코드 수
4. **출력 형식 선택** - CSV, JSON, SQL INSERT 또는 Python 스크립트
5. **현실적인 패턴 적용** - 데이터가 실제적이고 유효해 보이도록 설정
6. **비즈니스 제약 추가** - 비즈니스 로직 및 관계 준수
7. **데이터 생성 또는 스크립팅** - 실행 가능한 결과물 생성
8. **결과 검증** - 데이터 품질 및 완전성 확인

## 템플릿: Python 스크립트 출력

```python
import csv
import json
from datetime import datetime, timedelta
import random

# 설정
ROWS = $ROWS
FILENAME = "$DATASET_TYPE.csv"

# 현실적인 값 생성기를 포함한 열 정의
columns = {
    "id": "auto-increment",
    "name": "first_last_name",
    "email": "email",
    "created_at": "timestamp",
    # 추가 열...
}

def generate_dataset():
    """현실적인 더미 데이터셋 생성"""
    data = []
    for i in range(1, ROWS + 1):
        record = {
            "id": f"U{i:06d}",
            # 열 정의에 따른 값 생성
        }
        data.append(record)
    return data

def save_as_csv(data, filename):
    """데이터셋을 CSV로 저장"""
    with open(filename, 'w', newline='') as f:
        writer = csv.DictWriter(f, fieldnames=data[0].keys())
        writer.writeheader()
        writer.writerows(data)

if __name__ == "__main__":
    dataset = generate_dataset()
    save_as_csv(dataset, FILENAME)
    print(f"{FILENAME}에 {len(dataset)}개의 레코드가 생성되었습니다.")
```

## 예시 데이터셋 사양

**데이터셋 유형:** 고객 피드백

**열:**

- feedback_id (자동 증가, U001, U002...)
- customer_name (현실적인 이름)
- email (유효한 이메일 형식)
- feedback_date (지난 90일 이내의 날짜)
- rating (1-5 별점)
- category (버그, 기능 요청, 불만, 칭찬)
- text (현실적인 피드백 내용)
- product (전자제품, 의류, 홈데코)

**제약 조건:**

- 별점 분포: 5점 40%, 4점 30%, 3점 20%, 1-2점 10%
- 버그 카테고리는 별점 1-3점만 가능
- 기능 요청은 별점 3-5점만 가능
- 이메일 도메인 현실화 (gmail, yahoo, company.com 등)

## 출력물

- 즉시 실행 가능한 Python 스크립트 또는 직접적인 데이터 파일
- 적절한 헤더와 서식이 포함된 CSV 파일
- 유효한 구조와 유형을 갖춘 JSON 파일
- 데이터베이스 입력을 위한 SQL INSERT 문
- 데이터 유효성 검사 및 제약 조건 준수
- 현실적이고 비즈니스에 적합한 값
- 데이터 생성 로직에 대한 문서화
- 데이터셋 사용을 위한 빠른 시작 안내

## 출력 형식

**CSV:** 평면적인 테이블 형식으로, 스프레드시트나 데이터베이스로 가져오기 쉽습니다.

**JSON:** 계층적 구조로, API 및 NoSQL 데이터베이스에 적합합니다.

**SQL:** 관계형 데이터베이스에서 즉시 실행 가능한 INSERT 문입니다.

**Python 스크립트:** 사용자 정의 또는 대규모 데이터셋을 위한 실행 가능한 생성기입니다.
