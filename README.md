# E-commerce Backend

Kotlin과 Spring Boot 기반의 이커머스 백엔드 프로젝트입니다.
상품 조회, 주문·결제, 쿠폰·재고 관리부터 이벤트 처리와 상품 랭킹까지 구현하며 동시성 제어, 성능 개선, 장애 복구를 다룹니다.

프로젝트의 설계 의사결정, 비교한 대안과 트레이드오프는 **[Wiki에서 확인할 수 있습니다](https://github.com/0AndWild/E-commerce-Backend/wiki)**.
1~10주차별 설계 기록과 원본 PR을 함께 정리했습니다.

## 주차별 설계 기록

| 주차 | 설계 주제 | 원본 PR |
| --- | --- | --- |
| 1주차 | [회원 도메인과 비밀번호 정책](https://github.com/0AndWild/E-commerce-Backend/wiki/01%EC%A3%BC%EC%B0%A8-%E2%80%90-%ED%9A%8C%EC%9B%90-%EB%8F%84%EB%A9%94%EC%9D%B8%EA%B3%BC-%EB%B9%84%EB%B0%80%EB%B2%88%ED%98%B8-%EC%A0%95%EC%B1%85) | [#7](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/7) |
| 2주차 | [요구사항 중심 도메인 설계](https://github.com/0AndWild/E-commerce-Backend/wiki/02%EC%A3%BC%EC%B0%A8-%E2%80%90-%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD-%EC%A4%91%EC%8B%AC-%EB%8F%84%EB%A9%94%EC%9D%B8-%EC%84%A4%EA%B3%84) | [#21](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/21) |
| 3주차 | [상품 조회 모델과 페이징 정확성](https://github.com/0AndWild/E-commerce-Backend/wiki/03%EC%A3%BC%EC%B0%A8-%E2%80%90-%EC%83%81%ED%92%88-%EC%A1%B0%ED%9A%8C-%EB%AA%A8%EB%8D%B8%EA%B3%BC-%ED%8E%98%EC%9D%B4%EC%A7%95-%EC%A0%95%ED%99%95%EC%84%B1) | [#40](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/40) |
| 4주차 | [쿠폰과 재고의 동시성 제어](https://github.com/0AndWild/E-commerce-Backend/wiki/04%EC%A3%BC%EC%B0%A8-%E2%80%90-%EC%BF%A0%ED%8F%B0%EA%B3%BC-%EC%9E%AC%EA%B3%A0%EC%9D%98-%EB%8F%99%EC%8B%9C%EC%84%B1-%EC%A0%9C%EC%96%B4) | [#57](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/57) |
| 5주차 | [읽기 모델과 Redis 캐시 최적화](https://github.com/0AndWild/E-commerce-Backend/wiki/05%EC%A3%BC%EC%B0%A8-%E2%80%90-%EC%9D%BD%EA%B8%B0-%EB%AA%A8%EB%8D%B8%EA%B3%BC-Redis-%EC%BA%90%EC%8B%9C-%EC%B5%9C%EC%A0%81%ED%99%94) | [#78](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/78) |
| 6주차 | [비동기 결제와 멱등성 및 장애 복구](https://github.com/0AndWild/E-commerce-Backend/wiki/06%EC%A3%BC%EC%B0%A8-%E2%80%90-%EB%B9%84%EB%8F%99%EA%B8%B0-%EA%B2%B0%EC%A0%9C%EC%99%80-%EB%A9%B1%EB%93%B1%EC%84%B1-%EB%B0%8F-%EC%9E%A5%EC%95%A0-%EB%B3%B5%EA%B5%AC) | [#96](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/96) |
| 7주차 | [Outbox와 Kafka 이벤트 전달](https://github.com/0AndWild/E-commerce-Backend/wiki/07%EC%A3%BC%EC%B0%A8-%E2%80%90-Outbox%EC%99%80-Kafka-%EC%9D%B4%EB%B2%A4%ED%8A%B8-%EC%A0%84%EB%8B%AC) | [#106](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/106) |
| 8주차 | [주문 대기열과 입장 토큰 수명](https://github.com/0AndWild/E-commerce-Backend/wiki/08%EC%A3%BC%EC%B0%A8-%E2%80%90-%EC%A3%BC%EB%AC%B8-%EB%8C%80%EA%B8%B0%EC%97%B4%EA%B3%BC-%EC%9E%85%EC%9E%A5-%ED%86%A0%ED%81%B0-%EC%88%98%EB%AA%85) | [#116](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/116) |
| 9주차 | [Redis 기반 실시간 상품 랭킹](https://github.com/0AndWild/E-commerce-Backend/wiki/09%EC%A3%BC%EC%B0%A8-%E2%80%90-Redis-%EA%B8%B0%EB%B0%98-%EC%8B%A4%EC%8B%9C%EA%B0%84-%EC%83%81%ED%92%88-%EB%9E%AD%ED%82%B9) | [#137](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/137) |
| 10주차 | [기간 랭킹 배치와 안전한 결과 발행](https://github.com/0AndWild/E-commerce-Backend/wiki/10%EC%A3%BC%EC%B0%A8-%E2%80%90-%EA%B8%B0%EA%B0%84-%EB%9E%AD%ED%82%B9-%EB%B0%B0%EC%B9%98%EC%99%80-%EC%95%88%EC%A0%84%ED%95%9C-%EA%B2%B0%EA%B3%BC-%EB%B0%9C%ED%96%89) | [#144](https://github.com/loopers-labs/loop-pack-be-l2-vol4-kotlin/pull/144) |
