### JWT Passport TypeORM Exam
db : postgresql

```
jwt 토큰으로 인증 권한체크하는 예제
```

## Auth
```
@Post 회원가입
/auth/signup

"username" : "user",
"password" : '1234'

@Post 로그인
/auth/signin

"username" : "user",
"password" : '1234'
```

## Boards
```
@Get 나의 게시글 보기
/boards

Authorization Bearer Token : { access token }

@Get 게시글 보기
/boards/:id

@Post 게시글 작성
/boards/:id

Authorization Bearer Token : { access token }
"title" : "title",
"description" : "content"

@Delete 게시글 삭제
/boards/:id

Authorization Bearer Token : { access token }

@Patch 게시글 수정
/boards/:id/status

Authorization Bearer Token : { access token }
"status" : "PRIVATE" || "PUBLIC"
```

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](LICENSE).
