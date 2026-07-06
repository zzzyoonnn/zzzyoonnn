# 👋 Hi, I'm Jiyoon

Backend Engineer focused on transaction processing systems, payment architecture, and distributed backend applications.

Interested in building reliable financial systems that guarantee atomicity, consistency, and data integrity under high-concurrency environments.

Currently exploring:
- Java
- Spring Boot
- Kafka
- Payment Systems
- JVM Performance
- Distributed Systems

---

# 💳 FinFlow-backend

**Repository:** https://github.com/zzzyoonnn/FinFlow-backend

FinFlow is a backend project that simulates core banking operations with a focus on transactional integrity, consistency, and auditability. It explores how financial systems safely process deposits, withdrawals, and transfers while maintaining reliable account state.

Designed and implemented essential banking operations including:

- Deposit  
- Withdrawal  
- Transfer  
- Transaction history management  

## Key Contributions

- Designed withdrawal and transfer workflows within a single transactional boundary, guaranteeing atomic state changes across account and transaction entities.
- Applied domain-driven design principles by encapsulating business rules and invariants within the domain model, preventing invalid account states.
- Centralized request logging and execution monitoring using Spring AOP, reducing duplication across service components.
- Implemented transaction ledger recording with balance snapshots, enabling full traceability of account state changes and financial audits.
- Structured transaction processing flows into validation, state mutation, persistence, and response stages to improve maintainability and clarity.
- Eliminated N+1 query problems using Fetch Join, reducing database round-trips and improving transaction history retrieval performance by 30%.
- Deployed the application on AWS EC2 with MySQL hosted on Amazon RDS, establishing a production-like environment for end-to-end testing.

Through this implementation, I became particularly interested in how financial systems prevent data inconsistency, race conditions, and double execution under concurrent requests.

👉 Core Banking Service Implementation: [AccountService.java](https://github.com/zzzyoonnn/FinFlow-backend/blob/main/src/main/java/com/FinFlow/service/AccountService.java)


## 📝 Related Articles
- [계좌가 많아질 경우, 어떻게 설계하면 좋을까?🤔](https://zzzyoonnn.github.io/posts/2026/01/n+1/1/)
- [N+1은 왜 발생할까?🤔(Fetch Join 적용 전후 성능 비교)](https://zzzyoonnn.github.io/posts/2026/02/n+1/2/)
- [N+1은 왜 JPA에서 발생할까?🤔(JPQL)](https://zzzyoonnn.github.io/posts/2026/03/n+1/3/)
- [N+1은 메모리에 어떤 영향을 미칠까?🤔(JVM)](https://zzzyoonnn.github.io/posts/2026/03/n+1/4/)
- [영속성 컨텍스트는 N+1과 어떤 관계가 있을까?🤔(Hibernate)](https://zzzyoonnn.github.io/posts/2026/03/n+1/5/)
- [Fetch Join은 영속성 컨텍스트에서 어떻게 동작할까?🤔](https://zzzyoonnn.github.io/posts/2026/03/n+1/6/)
- [Hibernate 내부에서 영속성 컨텍스트는 어떻게 동작할까?🤔](https://zzzyoonnn.github.io/posts/2026/03/n+1/7/)
- [N+1은 GC를 왜 자주 발생시킬까?🤔](https://zzzyoonnn.github.io/posts/2026/01/n+1/8/)

---

# 🔄 Servlet2Spring

**Repository:** https://github.com/zzzyoonnn/Servlet2Spring

This project reflects my growth in understanding backend architecture evolution and framework-driven design.

Started with a JSP-based architecture and progressively evolved it into Spring MVC and Spring Boot.

## Key Contributions

- Replaced manual request handling and dependency management in Servlet-based architecture with Spring MVC and dependency injection, improving maintainability and testability.
- Migrated authentication from session-based login to Spring Security with JWT, improving scalability and decoupling authentication from server-side state.
- Integrated Spring Security to centralize authentication and authorization logic, reducing security-related code duplication.
- Deployed the migrated application on AWS using EC2, RDS, and S3, enabling cloud-native application management and deployment.

This migration process taught me the importance of modernizing systems **without compromising stability**, especially in environments where reliability is critical.

---

## 🛠 Tech Stack

**Backend**
- Java 21
- Spring Boot
- Spring Data JPA
- Spring Security (JWT)

**Database**
- MySQL
- H2 (for testing)

**Infrastructure**
- AWS (EC2, RDS, S3)

**Build Tool**
- Maven

---


# 🎯 Professional Interest

- Core Banking Systems  
- Transaction Processing  
- Financial Data Integrity  
- High-reliability Backend Systems  

---

# 💡 What I Aim to Build

I aim to build backend systems where correctness and reliability are prioritized over feature speed — especially in domains where data integrity is critical.
