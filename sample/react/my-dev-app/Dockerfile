# 사용할 기반 이미지 node.js 설치된 이미
FROM node:22-alpine

# 작업 디렉토리 경로
WORKDIR /app

# 파일복사  package.json 복사
COPY package.json . 

# 이미지 빌드 과정에서 수행하는 명령어
# 의존성 모듈 설치
RUN npm install

# 나머지 프로젝트 관련 소스 파일들 ... 복사
COPY . . 
# host경로 container경로
# source  destination

# 포트선언 (React 앱 기본포트 3000)
EXPOSE 3000

ENTRYPOINT ["npm", "start"]