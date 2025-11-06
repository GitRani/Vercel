# Mockup API 관리 및 배포를 위한 Vercel 실습

> Local Front Page에서 Create한 Mockup API를 Product Environment에서 사용하기 위한 Architecture 설계
> FastAPI, Docker-Compose, Vercel, Upstash(Redis), MySQL

- Vercel Hobby는 Request Limit가 큰 대신
Application이 무거우면 담을 수 없음.

- FastAPI 서버를 따로 띄워서 Vercel 셋팅

- 기존 Application에서 Route 요청 발생 시,
DB에 저장과 함께 DB에 저장된 Mockup API를 Upstash Redis에 Push

- Push된 API Lists를 배포된 Vercel 에서 사용 가능

