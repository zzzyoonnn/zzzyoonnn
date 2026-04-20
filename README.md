# 👋 Hi, I'm Jiyoon

Backend Developer focused on **transaction processing systems** and **core financial logic**.

I am interested in how financial systems guarantee **atomicity, consistency, and data integrity** under concurrent transaction environments.  
Through implementing core banking features and migrating legacy systems, I have developed a strong interest in building reliable and maintainable financial software.

---

# 💳 FinFlow-backend

**Repository:** https://github.com/zzzyoonnn/FinFlow-backend

A backend application that simulates core banking operations with a focus on transactional integrity.

Designed and implemented essential banking operations including:

- Deposit  
- Withdrawal  
- Transfer  
- Transaction history management  

## 🔎 Design Approach

- Managed withdrawal and transfer operations within a single `@Transactional` boundary to ensure **atomicity**
- Delegated validation logic (ownership, password verification, balance checks) to the **Account domain entity**
- Prevented negative balances through explicit business rule enforcement
- Recorded transaction history with **balance snapshots at the time of execution** for auditability
- Structured flow clearly as: **validation → state mutation → persistence → response**

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

## 🔎 Migration Focus

- Refactored the application into a clearer layered architecture
- Improved separation of concerns between controller, service, and domain layers
- Simplified configuration using Spring Boot auto-configuration
- Enhanced security structure using Spring Security
- Reduced boilerplate code and improved maintainability
- Improved deployment and dependency management with Maven

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
