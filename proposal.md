# Gsoc 

## **I. About Me**

**Name:** Shashwat Darshan\
**Email:** [shashwatdarshan153@gmail.com](mailto\:shashwatdarshan153@gmail.com)\
**GitHub:** [Shashwat-Darshan](https://github.com/Shashwat-Darshan)\
**Location:** New Delhi, India\
**Timezone:** GMT+5:30\
**Resume:** View Here

I am an enthusiastic software developer with a deep passion for backend technologies, system architecture, and high-performance computing. I have extensive hands-on experience with Python, Django, FastAPI, SQL, and containerization tools such as Docker. My technical foundation is built upon rigorous project-based learning and real-world applications, where I have successfully developed and optimized backend systems. Although my previous projects have been on a smaller scale, I am eager to undertake this significant migration project and work alongside experienced mentors at IHR to develop an efficient, high-performing, and maintainable backend architecture. I see this as an opportunity to further refine my technical capabilities, expand my problem-solving skills, and contribute meaningfully to an open-source initiative that impacts a global audience.

---

## **II. Why I Decided to Work for IHR**

I am thrilled at the prospect of contributing to the Internet Health Report (IHR) project because it presents a combination of complex technical challenges and a mission-driven approach that strongly aligns with my skills and values. The chance to migrate the IHR API from an outdated Django framework to the modern FastAPI, streamline database management using Bash scripts, and deploy the application efficiently through Docker aligns perfectly with my technical expertise in Django, FastAPI, SQL, and containerization technologies.

Beyond the technical aspects, I am deeply passionate about the project’s overarching goal of enhancing internet resiliency and accessibility—two critical components in today’s connected world. By participating in this initiative, I will have the opportunity to collaborate with a diverse and global developer community, gain invaluable hands-on experience in large-scale system migration, and contribute to an essential tool that informs and empowers millions. The combination of technical challenge, real-world impact, and professional growth makes this a compelling and deeply rewarding endeavor for me.

---

## **III. Project Title**

**Migrating IHR Backend from Django 2.2 to FastAPI for Improved Performance, Scalability, and Maintainability**

---

## **IV. Abstract**

The current IHR backend is built on Django 2.2.27, an outdated framework that lacks modern asynchronous capabilities. This limitation causes performance bottlenecks under high-concurrency conditions and makes the codebase increasingly difficult to maintain. Additionally, the existing system does not efficiently handle concurrent requests, leading to potential slowdowns during peak usage times.

My proposal is to migrate the IHR backend to FastAPI—a high-performance, asynchronous web framework designed for modern API development. This migration will significantly enhance API response times, simplify the system’s architecture, improve security, and auto-generate comprehensive API documentation using FastAPI’s native OpenAPI support. Furthermore, I will implement Bash scripts for database initialization, management, and schema migrations, as requested, to improve maintainability and streamline database operations. This transition will ultimately result in a faster, more scalable, and easier-to-maintain backend infrastructure, ensuring that the IHR project remains sustainable and adaptable to future demands.

---

## **V. Key Objectives and Motivation**

### **Key Objectives**

- **API Migration:** Migrate all Django API endpoints to FastAPI using asynchronous processing to reduce latency, increase throughput, and improve scalability.
- **Database Management:** Implement Bash scripts for database initialization, schema migrations, and management, ensuring efficient and maintainable database operations.
- **Containerization & Documentation:** Dockerize the FastAPI application for seamless deployment across different environments and auto-generate comprehensive API documentation using FastAPI’s built-in OpenAPI support.
- **Security Enhancements:** Implement robust authentication and request validation by integrating JWT-based authentication, OAuth2 endpoints, and role-based access control (RBAC) mechanisms.

### **Motivation for Migration**

- **Performance Bottlenecks:** The synchronous nature of Django’s views and ORM operations causes slow response times under heavy loads. Asynchronous processing in FastAPI will allow the system to handle a larger number of concurrent requests more efficiently.
- **Maintainability Issues:** The current monolithic codebase is complex and difficult to maintain. Adopting a modular design with type-safe models will simplify the code and improve long-term maintainability.
- **Scalability Constraints:** As data volume grows and user demand increases, the existing Django-based architecture struggles to scale. FastAPI’s support for asynchronous requests, combined with optimized database interactions, will significantly enhance the system’s scalability.
- **Security Enhancements:** The modernization process will introduce more secure authentication mechanisms, such as JWT and OAuth2, to protect user data and enforce better access control policies.

---

## **VI. Expected Outcomes**

- **Substantial improvements in API performance** through asynchronous request handling and optimized query execution.
- **A more modular, maintainable, and scalable backend architecture** that is easier to extend and optimize in the future.
- **Enhanced developer experience** through automatic API documentation, type safety, and better error handling.
- **Stronger security measures** with JWT-based authentication, OAuth2 support, and improved input validation techniques.
- **Improved system resilience and fault tolerance**, ensuring the IHR API can handle increasing workloads efficiently.
- **Database Management**, Efficient and maintainable database management through the use of Bash scripts for initialization, migrations, and operations.
    
## **Suggested Enhancements for Discussion**

While the core migration plan aligns with mentor guidance, additional improvements could further enhance the system’s efficiency and security. These could be proposed as stretch goals:

### **Potential Enhancements:**

- **SQLAlchemy + Alembic for Database Management:** While Bash scripts are preferred for simplicity, an alternative approach using SQLAlchemy ORM could improve query flexibility and migrations.
- **Advanced Caching with Redis:** Implementing Redis as a caching layer can optimize API response times by reducing redundant queries and improving data retrieval efficiency.
- **Asynchronous Task Processing:** Utilizing Celery with FastAPI for background tasks such as email notifications, scheduled data updates, and long-running computations to improve system responsiveness.
- **Enhanced Authentication:** Introducing OAuth2-based authentication alongside JWT for greater security, compliance with modern standards, and improved user access management.

These enhancements will be discussed with mentors to assess feasibility and prioritize implementation based on project goals and available resources.

---

## **VII. Deliverables and Timeline**

## **Project Deliverables**

### Code Migration:

- Migrate all Django views and API endpoints to FastAPI with async support.
- Implement structured request handling and response validation using Pydantic models.
- Convert Django ORM-based database interactions to SQLAlchemy v2.0 for improved efficiency.
- Manage database schema changes and versioning with Alembic.

### **Security Enhancements:**

- Implement secure JWT-based authentication with optional OAuth2 support.
- Introduce role-based access control (RBAC) to enforce user permissions effectively.
- Strengthen input validation and enforce security best practices.
- Implement rate limiting and security headers middleware for additional protection.

### **Performance Optimizations:**

- Introduce caching mechanisms such as Redis to optimize frequently accessed database queries.
- Conduct load testing to identify and eliminate performance bottlenecks.
- Implement database connection pooling and asynchronous query execution for better resource utilization.
- Integrate Celery for handling background tasks asynchronously.

### **Deployment and Containerization:**

- Containerize the FastAPI application using Docker for efficient deployment.
- Develop CI/CD workflows to automate testing and deployment pipelines.
- Enhance logging and monitoring with OpenTelemetry to track system performance and error rates.

### **Documentation and Testing:**

- Maintain comprehensive project documentation, including migration guides, API documentation, and system architecture details.
- Implement extensive test coverage using pytest and pytest-asyncio for robustness.
- Conduct security and performance audits to validate the migration’s success.
- Auto-generate API documentation with FastAPI’s OpenAPI support for developer ease-of-use.

## **Timeline and Implementation Plan**

## **Community Bonding (May 8 - June 1, 2025)**

### **Goals:**
- Understand the existing Django 2.2 codebase in detail.
- Engage with mentors and discuss migration strategies.
- Document current API behavior, dependencies, and challenges.
- Define key milestones and deliverables.

### **Tasks:**
- Study and analyze existing models (`models.py`) including `Hegemony`, `ASN`, `Country`, and database caching strategies.
- Review API endpoints in `views.py` such as network monitoring and hegemony analysis.
- Document authentication methods, database relationships, and performance bottlenecks.
- Prepare a high-level migration roadmap with mentors.

### **Challenges:**
- Understanding complex business logic in Django models.
- Identifying potential pitfalls in migrating monolithic components.

---

## **Migration Strategy**

### **1. Parallel Development Approach**
```markdown
Current Setup:
- Django 2.2.27 (Production)
└── FastAPI (Development)
    - Run both systems in parallel
    - Gradually shift traffic
    - Ensure zero downtime
```

### **2. Component-wise Migration**

#### **Database Layer**
```python
from sqlalchemy import Column, Integer, String
from sqlalchemy.ext.declarative import declarative_base

Base = declarative_base()

class Hegemony(Base):
    __tablename__ = "hegemony"
    id = Column(Integer, primary_key=True)
    asn = Column(Integer)
    # ...existing model fields...
```

#### **API Endpoints**
```python
from fastapi import APIRouter, Depends
from typing import List

router = APIRouter()

@router.get("/hegemony/", response_model=List[HegemonyResponse])
async def get_hegemony(timebin: str = None):
    # Migrate existing Django view logic to async
    # ...existing business logic...
```

### **3. Migration Phases**

```markdown
1. Setup & Infrastructure (2 weeks)
   - FastAPI project structure
   - Database connection setup
   - Authentication framework

2. Core Features (3 weeks)
   - Models migration
   - Essential endpoints
   - Basic authentication

3. Advanced Features (4 weeks)
   - Complex queries
   - Caching implementation
   - WebSocket support

4. Testing & Optimization (2 weeks)
   - Performance testing
   - Security auditing
   - Documentation
```

### **4. Key Components to Migrate**

```markdown
1. Database Models:
   - Hegemony
   - ASN
   - Country
   - Network Delay

2. API Endpoints:
   - /hegemony/
   - /hegemony/countries/
   - /hegemony/asns/
   - User management endpoints

3. Authentication:
   - Token-based auth → JWT
   - User sessions
   - Permissions
```

### **5. Technical Considerations**

```python
# Requirements
fastapi>=0.100.0
sqlalchemy>=2.0.0
pydantic>=2.0.0
alembic>=1.11.0
asyncpg>=0.28.0
python-jose[cryptography]
passlib[bcrypt]
```

---

## **Phase 1: Core Setup (June 2 - June 15, 2025)**

### **Goals:**

- Set up the FastAPI project structure.
- Establish core middleware, request handling, and database connections.
- Migrate initial API endpoints to ensure a functional base.

### **Tasks:**

- Create FastAPI project skeleton:
  ```plaintext
  ihr_fastapi/
  ├── app/
  │   ├── core/
  │   │   ├── config.py      # Configuration management
  │   │   └── security.py    # Authentication setup
  │   ├── api/
  │   │   └── v1/           # API versioning
  │   ├── models/           # SQLAlchemy models
  │   └── schemas/          # Pydantic models
  ```
- Implement environment configurations for PostgreSQL, Redis caching, and authentication.
- Set up Docker containers for FastAPI, PostgreSQL, and Redis.
- Establish initial API endpoints and middleware.

### **Challenges:**

- Ensuring a seamless transition of configurations from Django settings.
- Handling initial API requests asynchronously.

---

## **Phase 2: Data Models Migration (June 16 - July 5, 2025)**

### **Goals:**

- Migrate Django models to SQLAlchemy ORM.
- Optimize database operations for async execution.
- Implement Alembic migrations.

### **Tasks:**

- Convert Django models into SQLAlchemy models:
  - Migrate `Hegemony_country`, `Hegemony_prefix`, `Atlas_delay`, `TR_hegemony`.
  - Adapt complex relationships and optimize query execution.
- Implement Alembic-based schema migrations.
- Integrate caching optimizations for frequently accessed models.

### **Challenges:**

- Ensuring database integrity and migration correctness.
- Handling large datasets efficiently.

---

## **Phase 3: API Migration (July 6 - July 25, 2025)**

### **Goals:**

- Convert key Django API views into FastAPI.
- Implement async request handling.
- Ensure feature parity.

### **Tasks:**

- Migrate Django API views to FastAPI.
- Implement request validation and response models using Pydantic.
- Validate API behavior against the existing Django system.

### **Challenges:**

- Maintaining API consistency.
- Handling unexpected behavior in async execution.

---

## **Phase 4: Authentication & Security (July 26 - August 5, 2025)**

### **Goals:**

- Implement JWT & OAuth2 authentication.
- Migrate permission models.
- Enforce security enhancements.

### **Tasks:**

- Replace Django authentication with FastAPI OAuth2 & JWT.
- Migrate user roles and permissions.
- Implement security best practices (rate limiting, input validation).

### **Challenges:**

- Ensuring a seamless transition without breaking authentication workflows.
- Strengthening security while maintaining usability.

---

## **Phase 5: Optimization & Deployment (August 6 - August 15, 2025)**

### **Goals:**

- Implement Redis caching, WebSocket support, and performance benchmarking.
- Dockerized deployment.
- Final API documentation.

### **Tasks:**

- Optimize query performance with async execution.
- Implement Redis-based caching for frequently accessed APIs.
- Enable WebSocket support for real-time data streaming.
- Finalize API documentation using OpenAPI.
- Deploy using Docker and Kubernetes.

### **Challenges:**

- Ensuring performance optimizations are effective.
- Finalizing deployment strategies without disrupting service.

---

## **Final Evaluation (August 16 - August 25, 2025)**

### **Goals:**

- Validate migration success.
- Perform final testing and documentation updates.
- Submit final deliverables.

### **Tasks:**

- Conduct integration tests to verify API functionality.
- Perform final load testing (simulate high traffic volumes).
- Document migration steps for future maintainability.
- Ensure FastAPI’s OpenAPI documentation is accurate and user-friendly.
- Gather mentor feedback and incorporate final refinements.

### **Challenges:**

- Ensuring all edge cases are tested and accounted for.
- Completing final refinements within the timeline.

---

##



| **Phase**                     | **Tasks** | **Timeline** |
|-------------------------------|----------|-------------|
| **Community Bonding** | Engage with mentors, analyze the Django 2.2 codebase, document existing API behavior, dependencies, and challenges. | **May 8 - June 1, 2025** |
| **Phase 1: Core Setup** | Establish FastAPI project structure, set up database connections, middleware, authentication, and initial API endpoints. | **June 2 - June 15, 2025** |
| **Phase 2: Data Models Migration** | Convert Django models to SQLAlchemy, implement async queries, optimize database interactions, and integrate Alembic migrations. | **June 16 - July 5, 2025** |
| **Phase 3: API Migration** | Convert key Django API views into FastAPI, implement async request handling, ensure feature parity. | **July 6 - July 25, 2025** |
| **Phase 4: Authentication & Security** | Implement JWT & OAuth2 authentication, migrate permission models, and enforce security enhancements. | **July 26 - August 5, 2025** |
| **Phase 5: Optimization & Deployment** | Redis caching, WebSocket support, performance benchmarking, Dockerized deployment, final API documentation. | **August 6 - August 15, 2025** |
| **Final Evaluation** | Testing, bug fixes, mentor reviews, performance audits, final documentation submission. | **August 16 - August 25, 2025** |

### **VIII. Unit Testing Strategy**

A robust testing framework is crucial for the success of this migration. The testing strategy will include:

- **Framework:** Utilize `pytest` along with `pytest-asyncio` to support asynchronous testing.
- **API Testing:** Validate that each FastAPI route behaves as expected and meets performance benchmarks.
- **Database Testing:** Ensure data integrity post-migration by comparing outcomes with baseline results from the current Django system.
- **Performance Testing:** Conduct load tests to confirm that the new endpoints achieve response times below 100ms.
- **Security Testing:** Validate the effectiveness of the new authentication mechanisms and error-handling routines.

Each test case will be thoroughly documented, with fixtures set up to simulate the necessary environments and ensure reproducibility.

## **IX. Expectations from Mentor**

I am always looking to learn and improve upon my mistakes. I would like my mentors to provide constructive feedback, so we can work together to make my project better. This gives me the opportunity to collaborate with them and learn from their experiences as professionals in this field. I would also love to understand their motivations for working with the IHR and learn about their career journeys.

## **X. Other Commitments**

During the GSoC period, my primary focus will be on this project. I do not have any full-time commitments that would interfere with my ability to complete the expected deliverables. However, I may occasionally work on personal development projects or engage in my college studies, especially during exam periods.

## **XI. Future Plans After GSoC**

After the GSoC period is over, I plan to continue contributing to the IHR project by maintaining and improving the backend infrastructure. I am also interested in exploring opportunities in backend system architecture, distributed computing, and cloud-native development. Additionally, I would love to mentor future GSoC participants and help them navigate the program, as I will have firsthand experience of the challenges and learning opportunities it offers.

---

