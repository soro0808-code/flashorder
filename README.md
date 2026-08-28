# flashorder

DB 동시성 재현기. 재고 1개를 두 명이 동시에 사는 순간을 한 틱씩 재생합니다.

https://soro0808-code.github.io/flashorder/

PostgreSQL 17.11에서 실제로 재현한 Lost Update와 데드락을 타임라인·코드·세션 로그로 나란히 봅니다. 시나리오는 락 없음, 비관적 락(SELECT ... FOR UPDATE), 낙관적 락(@Version), 원자적 UPDATE, 데드락 다섯 가지입니다.

글: https://seungwon08.tistory.com
