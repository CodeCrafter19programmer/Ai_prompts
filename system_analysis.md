You are conducting a FULL production-readiness audit of an online store system.

Assume the following roles simultaneously and analyze the system from each perspective:

1. End User (Buyer/Seller)
2. Security Administrator
3. Database Administrator
4. System Analyst
5. DevOps Engineer
6. Senior Software Architect

Your task is to perform a COMPLETE system audit including:

1. CODE REVIEW
- Analyze backend and frontend code quality
- Identify bad practices, technical debt, and performance issues
- Check for security vulnerabilities (SQL injection, XSS, CSRF, authentication flaws)
- Verify input validation and error handling
- Evaluate modularity, scalability, and maintainability
- Suggest production-grade improvements

2. SYSTEM ARCHITECTURE ANALYSIS
- Review folder structure and project organization
- Evaluate separation of concerns (MVC or similar pattern)
- Check API structure and routing
- Identify scalability limitations
- Recommend industry-standard architecture improvements

3. DATABASE AUDIT
- Analyze database schema design
- Check normalization and indexing
- Identify redundant or inconsistent fields
- Review relationships, constraints, and data integrity
- Suggest improvements for performance and scalability

4. SECURITY AUDIT
Act as a security engineer and attempt to break the system logically:
- authentication weaknesses
- authorization flaws
- insecure file uploads
- session management issues
- password storage practices
- rate limiting
- data exposure risks

Provide mitigation strategies for each vulnerability.

5. USER EXPERIENCE REVIEW
Pretend to be an actual buyer and seller using the store:
- analyze navigation flow
- checkout or product posting process
- usability problems
- trust and credibility signals
- mobile responsiveness

6. DEVOPS & DEPLOYMENT REVIEW
Evaluate whether the system is production ready:
- environment configuration
- logging and monitoring
- backup strategy
- scalability
- caching
- CDN usage
- containerization or deployment pipeline
- error tracking

7. PERFORMANCE ANALYSIS
Identify:
- slow database queries
- inefficient loops
- unnecessary API calls
- frontend performance issues

Provide optimization recommendations.

8. PRODUCTION READINESS SCORE
Give a score from 1–100 for:
- security
- scalability
- maintainability
- performance
- architecture quality

9. ACTION PLAN
Provide a prioritized roadmap:
- critical issues (must fix before launch)
- important improvements
- optional optimizations

Important:
Be extremely critical and assume the system will handle thousands of users and real payments.

Respond with structured sections and clear recommendations.

I will provide the project files, folder structure, and database schema for analysis.
