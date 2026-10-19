# 임채륜 | Backend Engineer

반복되는 문제를 원인부터 찾아, 다시 일어나지 않는 구조로 끝내는 백엔드 엔지니어입니다.
고쳤다고 말하기 전에 재현하고, 고친 뒤에는 재발하지 않는지 확인합니다.

- Blog: [velog.io/@publeman](https://velog.io/@publeman/posts)
- Email: dlacofbs1229@gmail.com

## 문제 해결 기록

| 문제 | 해결 | 결과 |
|---|---|---|
| 매주 반복되던 시스템 간 재고 불일치 (실무, ERP·MES) | 수불 로그 5일치로 원인 추적, 마스터 코드 정비, MSSQL 프로시저 4건 수정, 3주간 재발 확인 | 수동 수정 요청 주 4건 → **0건** |
| 동시 요청 시 크레딧 차감 누락 ([HOUME](https://github.com/TEAM-HOUME/HOUME-SERVER)) | JMeter로 재현 → Redisson 분산락 적용 → 같은 테스트로 재검증 | 차감 누락 재발 없음 |
| 외부 AI 서버 장애가 서비스 전체로 전파 ([HOUME](https://github.com/TEAM-HOUME/HOUME-SERVER)) | Sentry로 발견 → 서킷 브레이커로 차단 | 관련 오류 **95% 감소** |
| 조회 API 응답 지연 ([HOUME](https://github.com/TEAM-HOUME/HOUME-SERVER)) | Grafana로 발견 → traceId 로그로 원인 추적 → 캐시 적용 | **200ms → 20ms** |
| 재연결 시 실시간 알림 유실 ([MediHub](https://github.com/PBEM22/medihub)) | SSE Last-Event-ID 이후 이벤트 재전송 | 알림 유실 **0건** |
| 다중 파드 환경 세션 불일치 ([MediHub](https://github.com/PBEM22/medihub)) | Redis 세션 클러스터링 | 파드 변경 시에도 로그인 유지 |
| 열린 PR에 미검증 커밋이 섞이던 배포 사고 ([MediHub](https://github.com/PBEM22/medihub)) | release 단계 도입, GitHub Actions로 PR 생성 자동화 | PR 동기화 오류 **0건**, 버전별 롤백 |

## 프로젝트
- **[HOUME](https://github.com/TEAM-HOUME/HOUME-SERVER)** · AI 인테리어 이미지 생성 서비스 · 백엔드 (2025.06 ~ 현재) · [houme.kr](https://houme.kr)
- **[MediHub](https://github.com/PBEM22/medihub)** · 병원 지식관리 서비스 · 팀장, 백엔드·인프라 (2024.11 ~ 2025.01)
- **[POTI](https://github.com/team-poti/POTI-SERVER)** · K-pop 굿즈 공동구매 앱 · 백엔드 리드 (2025.12 ~ 현재) · iOS·Android 출시

## 기술
- **Backend** Java, Spring Boot, Spring Security, JPA, QueryDSL
- **Data** MySQL, MariaDB, PostgreSQL, Redis
- **Infra** Docker, Kubernetes(EKS), AWS, ArgoCD, GitHub Actions, Nginx, Terraform
- **Observability** Prometheus, Grafana, Sentry

<!-- <div align="center">
  
![PBEM22](https://capsule-render.vercel.app/api?type=venom&color=auto&height=300&section=header&text=임채륜%20&fontSize=50)  

  <h2>협업과 개발 생산성을 중시하는 엔지니어 임채륜입니다.</h2> 
   
<a href="https://github.com/devxb/gitanimals">
<img
  src="https://render.gitanimals.org/farms/PBEM22"
  width="600"
  height="300"
/>
</a>

<br>
<h2>☑️ Use Stack </h2>
<h4>🖥️ Front-End </h4>
<img src="https://img.shields.io/badge/html-E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" /> <img src="https://img.shields.io/badge/css-4574E0.svg?style=for-the-badge&logo=css3&logoColor=white" /> <img src="https://img.shields.io/badge/javascript-F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=20232a" /> <img src="https://img.shields.io/badge/react-20232a.svg?style=for-the-badge&logo=react&logoColor=61DAFB" /> <img src="https://img.shields.io/badge/Vue-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white">
  

<h4>💻 Back-End </h4>
<img src="https://img.shields.io/badge/java-F44336.svg?style=for-the-badge&logo=java&logoColor=white" /> <img src="https://img.shields.io/badge/spring-8BC34A.svg?style=for-the-badge&logo=spring&logoColor=white" /> <img src="https://img.shields.io/badge/security-20232a.svg?style=for-the-badge&logo=springsecurity&logoColor=6DB33F" /> <img src="https://img.shields.io/badge/spring boot-6DB33F.svg?style=for-the-badge&logo=springboot&logoColor=white" /> <img src="https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white" />

<img src="https://img.shields.io/badge/mariadb-003545.svg?style=for-the-badge&logo=mariadb&logoColor=white" />     

<!-- <img src="https://img.shields.io/badge/docker-1488C6.svg?style=for-the-badge&logo=docker&logoColor=white" /> <img src="https://img.shields.io/badge/jenkins-D24939.svg?style=for-the-badge&logo=jenkins&logoColor=white" /> --> 
<!--
<h2>🛠️ Tool's </h2>
<img src="https://img.shields.io/badge/notion-white.svg?style=for-the-badge&logo=notion&logoColor=black" /> <img src="https://img.shields.io/badge/git-F14232.svg?style=for-the-badge&logo=git&logoColor=white" />
 <img src="https://img.shields.io/badge/github-181717.svg?style=for-the-badge&logo=github&logoColor=white" />  <img src="https://img.shields.io/badge/intellij-20232a.svg?style=for-the-badge&logo=intellijidea&logoColor=white" /> 
 

<h2>🌈 Contact</h2>
<a href="https://velog.io/@publeman">
  <img src="https://img.shields.io/badge/velog-1EBC8F.svg?style=for-the-badge&logo=velog&logoColor=white" />
</a>
<!-- <a href="https://www.discord.com/users/323169081908002818">
  <img src="https://img.shields.io/badge/discord-7289DA.svg?style=for-the-badge&logo=discord&logoColor=white" />
</a> -->
<!-- <a href="https://www.instagram.com/dlacofbs/">
  <img src="https://img.shields.io/badge/instagram-E4405F.svg?style=for-the-badge&logo=instagram&logoColor=white" />
</a> -->
<!--
<a href="mailto:dlacofbs1229@gmail.com">
  <img src="https://img.shields.io/badge/dlacofbs1229@Gmail.com-D14836.svg?style=for-the-badge&logo=gmail&logoColor=white" /> 
</a>

<br>
<br>
<br>
<br>

<h2> 🧮 Status </h2>

<!-- ![PBEM's GitHub stats](https://github-readme-statss-wine.vercel.app/api?username=PBEM22&show_icons=true&theme=dark) -->
<!--
<br>

[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=dlacofbs)](https://solved.ac/dlacofbs/)

</div>
-->
