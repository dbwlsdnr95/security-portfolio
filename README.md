# 📜 유진욱 포트폴리오

> Penetration Tester & Security Engineer  
> 모의해킹 · 취약점 분석 · CVE PoC · 클라우드 보안(Akamai / AWS / GCP)

<br />

# 👋 Intro

> 보안운영 경험을 기반으로  
> 현재는 **웹·모바일 진단, CVE PoC 연구, Cloud 보안** 에 집중하고 있습니다.  
> 실제 서비스 취약점 분석부터 PoC 재현, 공격 로그 기반 대응 전략 수립까지  
> **"재현 → 분석 → 대응" 전 과정**을 수행하는 보안 엔지니어를 목표로 합니다.

<br />

# 📝 Projects

아래 프로젝트들은 **실제 기업 환경 기반 연구**,  
또는 **실습 환경을 직접 구축하여 공격·방어를 검증한 프로젝트**들입니다.

<br />

---
# 1. 🧨 CVE Research (KEV 기반 PoC 분석)

### CVE-2022-22965 – Spring4Shell RCE PoC 재현

**수행 목적**  
- 실제 고객사 자산과 연관된 CVE 위협 분석  
- 취약 환경을 직접 구축하여 RCE 가능성 검증  

**담당 역할**  
- Docker 기반 Spring Boot 취약 환경 구성  
- 악성 파라미터를 이용한 RCE PoC 실행  
- Log 기반 공격 흐름 분석 및 영향 범위 정리  

**주요 성과**  
- KEV(Spring4Shell) 취약점 실제 재현 성공  
- 패치 적용 후 RCE 차단(404 Redirect) 검증  
- 대응 가이드 및 예방 정책 문서화  

🔗 **[프로젝트 상세 보기](./cve-research)**

<br /><br />

---

# 2. 🌐 Web Application Security Assessment

**수행 목적**  
- 실제 서비스와 유사한 웹 환경을 직접 구축하여 취약점 발생 구조를 이해  
- SQLi · XSS · SSRF 등 핵심 취약점을 인위적으로 생성하고 공격 재현  
- 취약점 수정 전·후의 보안성 차이를 실제 실습으로 검증  

**담당 역할**  
- 취약한 Web/API 구조 직접 설계 및 구현  
- SQLi/XSS/File Downlod/File Upload 기반 공격 시나리오 작성 및 실제 PoC 수행  
- 식별된 취약점 분석 후 원인 파악 및 코드 레벨 보안 패치 적용  
- 이후 재공격을 통해 패치 효과 검증  
- 회사 ASM 솔루션에서 동일 공격이 어떻게 진행되는지 확인  

**주요 성과**  
- 직접 구축한 웹에서 다수의 고위험 취약점 재현 성공  
- 취약점 패치 후 재검증을 통해 보안성 향상 확인  
- 회사 ASM 탐지 과정 분석을 통해 실제 실무 환경에서의 탐지·우회 가능성 이해 확보
  
🔗 **[프로젝트 상세 보기](./web/web-hacking)**

---

# 3. 📱 Mobile Security Testing

**수행 목적**  
- 모바일 앱의 API 구조 분석 및 취약점 식별  
- 인증 및 세션 검증 로직 우회 가능성 확인  

**담당 역할**  
- APK 디컴파일 및 코드 분석  
- Frida 기반 함수 후킹 및 변수 조작  
- Burp MITM 환경에서 HTTPS 우회 및 API 분석  

**주요 성과**  
- 인증/세션 로직 취약점 발견  
- 모바일 API 보안성 개선 방향 제안

🔗 **[프로젝트 상세 보기](./web/mobile-security)**

---

# 4. 💻 System Hacking Project

**수행 목적**  
- Linux 환경에서 권한 상승 가능성을 실습으로 검증  
- 실제 공격 체인(Low → Root)을 단계별로 재현  

**담당 역할**  
- 취약한 Linux Lab 구성  
- SUID, Cron, PATH Hijacking, Capabilities 등 PrivESC 수행  
- 공격 흐름 및 로그 기반 원인 분석  

**주요 성과**  
- 다양한 권한상승 기법 재현 성공  
- 공격 시나리오 기반 대응 가이드 작성  


🔗 **[프로젝트 상세 보기](./system/linux-privesc)**

---

# 5. ☁ Cloud WAF Testing & Detection Analysis

**수행 목적**  
- 사내 개발 중인  WAF테스터 기반으로 Cloud WAF의 탐지 성능 비교  
- Akamai / AWS / Cloudflare / MonitorsLab의 정책 차이 분석  

**담당 역할**  
- 여러 공격 자동화 테스트  
- WAF별 탐지·미탐지 결과 수집  
- 로그 기반 정책 차이 분석  

**주요 성과**  
- 4개 솔루션 탐지 성향 비교표 작성  
- 미탐지 패턴 식별 및 정책 보완 포인트 도출  
- 서비스 보안 운영 시 선택 기준 제시  

🔗 **[프로젝트 상세 보기](./cloud/waf-testing)**  

---

# 6. 🛡 ISO 27001 기반 보안 운영

**수행 목적**  
- ISO 27001 기준에 맞는 보안 운영 프로세스 구축  
- 인증 대비 보안 취약 요소 개선  

**담당 역할**  
- 내부 보안 점검 수행  
- 보안솔루션 정책 검토 및 개선
- 보안솔루션 인프라 진단 점검  

**주요 성과**  
- ISO 기반 운영 문서 정리  
- 웹/네트워크 보안 정책 정비  
- 내부 보안성 강화 기여  

🔗 **[프로젝트 상세 보기](./iso)**

---

# 📞 Contact

- Email : **wlsdnr255@naver.com**  
- GitHub : https://github.com/dbwlsdnr95
