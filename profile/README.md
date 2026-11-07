<!--
  ZIUAI organization profile
  Repo: github.com/ziuai-ai-tech/.github  ->  file: profile/README.md  (images in profile/assets/)
  If your organization username is not "ziuai", replace "ziuai" in every image URL below.
-->

<p align="center">
  <img src="https://raw.githubusercontent.com/ziuai-ai-tech/.github/main/profile/assets/header.svg" width="100%" alt="ZIUAI | Engineering & Technology — Building Intelligent Solutions Through Engineering Excellence"/>
</p>

<h3 align="center">Welcome to the official GitHub organization of ZIUAI.</h3>

<p align="center">
  We build software products, AI-powered applications, automation solutions and scalable technology platforms.<br/>
  Our engineering approach focuses on <b>quality</b>, <b>security</b>, <b>maintainability</b>, <b>performance</b> and <b>continuous improvement</b>.<br/>
  This organization is the central workspace for our engineering projects and collaborative development.
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ziuai-ai-tech/.github/main/profile/assets/divider.svg" width="100%" alt=""/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ziuai-ai-tech/.github/main/profile/assets/principles.svg" width="100%" alt="Our Engineering Principles: Code Quality, Security First, Scalability, Reliability, Collaboration, Continuous Improvement"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ziuai-ai-tech/.github/main/profile/assets/teams.svg" width="100%" alt="Technology and Engineering Teams: Frontend, Backend, AI/ML, Automation, QA, DevOps, Technical Management"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ziuai-ai-tech/.github/main/profile/assets/pipeline.svg" width="100%" alt="How we ship: Task, Branch, Implement, Test, Commit, Pull Request, Review, Merge, Release"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ziuai-ai-tech/.github/main/profile/assets/standards.svg" width="100%" alt="Development Standards"/>
</p>

<details>
<summary><b>01 &nbsp;·&nbsp; Account & Organization Guidelines</b></summary>
<br/>

- Use your approved professional company email for organization membership.
- Every team member must use their own GitHub account.
- Enable **Two-Factor Authentication (2FA)**.
- Never share passwords, authentication codes or recovery codes.
- Do not transfer company code into personal repositories.
- Follow assigned repository and team permissions.

</details>

<details>
<summary><b>02 &nbsp;·&nbsp; Repository Management</b></summary>
<br/>

- Use meaningful and consistent repository names.
- Keep project documentation updated.
- Include a `README.md` in every project repository.
- Maintain an appropriate `.gitignore` file.
- Do not commit build artifacts, temporary files or unnecessary dependencies.
- Keep company source code in authorized organization repositories.

</details>

<details>
<summary><b>03 &nbsp;·&nbsp; Branching Strategy</b></summary>
<br/>

| Branch | Purpose |
|---|---|
| `main` | Production-ready code |
| `development` | Integrated development |
| `feature/*` | New feature development |
| `bugfix/*` | Bug fixes |
| `hotfix/*` | Urgent production fixes |
| `release/*` | Release preparation |

**Examples:** `feature/user-authentication` · `feature/ai-document-processing` · `bugfix/api-validation` · `hotfix/production-error` · `release/v1.2.0`

> **Direct pushes to protected production and development branches are not permitted.**

</details>

<details>
<summary><b>04 &nbsp;·&nbsp; Pull Request Guidelines</b></summary>
<br/>

All code changes must be submitted through **Pull Requests**.

**Every Pull Request should include:**
- A clear and meaningful title
- Description of the changes
- Related task or issue ID
- Implementation details
- Testing performed
- Screenshots for UI changes, where applicable
- Potential impact on APIs, databases and integrations

**Before merging:**
- Required code reviews must be completed
- All required CI/CD checks must pass
- Review comments must be resolved
- Required approvals must be obtained

</details>

<details>
<summary><b>05 &nbsp;·&nbsp; Coding Standards</b></summary>
<br/>

**General Coding Practices**
- Write clean, readable and maintainable code.
- Follow the language-specific formatting and linting standards.
- Use meaningful variable, function and class names.
- Avoid duplicate code and unnecessary complexity.
- Keep functions and modules focused on specific responsibilities.
- Handle exceptions and errors properly.
- Avoid hardcoded configuration values.
- Remove unused imports, debugging statements and dead code.
- Add comments where business logic requires clarification.
- Write appropriate unit and integration tests.

**Code Organization**
- Follow the established project architecture.
- Separate business logic, presentation and data-access layers appropriately.
- Use reusable components and shared utilities.
- Maintain consistent folder structures.
- Update technical documentation when architecture or functionality changes.

**Code Review** — every contributor must:
- Review code carefully before submitting a PR.
- Provide constructive and professional feedback.
- Check functionality, readability, security and performance.
- Avoid approving code without understanding the changes.

</details>

<details>
<summary><b>06 &nbsp;·&nbsp; AI & Machine Learning Development Standards</b></summary>
<br/>

AI and ML projects require additional validation and responsibility.

- Maintain version-controlled prompts and model configurations.
- Document model names, versions and important parameters.
- Validate AI-generated code before merging.
- Evaluate model accuracy, reliability and consistency.
- Maintain relevant test cases and evaluation datasets.
- Monitor model performance and unexpected outputs.
- Protect confidential datasets and customer information.
- Never commit API keys, tokens or production credentials.
- Follow approved AI services and data-handling policies.

</details>

<details>
<summary><b>07 &nbsp;·&nbsp; API & Integration Guidelines</b></summary>
<br/>

- Follow consistent API naming conventions.
- Use appropriate HTTP status codes.
- Validate incoming requests.
- Implement proper authentication and authorization.
- Handle errors consistently.
- Document API contracts and integration requirements.
- Maintain backward compatibility where required.

</details>

<details>
<summary><b>08 &nbsp;·&nbsp; Security & Data Protection</b></summary>
<br/>

> **Security is everyone's responsibility.**

**Never commit or publish:**
- API keys and access tokens
- Passwords and authentication credentials
- Private certificates and secret keys
- Confidential customer documents
- Personally identifiable information
- Proprietary datasets or restricted business information

**Additional requirements:**
- Store secrets using approved secret-management solutions.
- Review third-party dependencies for vulnerabilities.
- Follow least-privilege access principles.
- Report security vulnerabilities through authorized company channels.
- Do not expose internal infrastructure or production configurations publicly.

</details>

<details>
<summary><b>09 &nbsp;·&nbsp; Testing & Quality Assurance</b></summary>
<br/>

- Developers must test their changes before submitting PRs.
- Write unit tests for appropriate business logic.
- Perform integration testing for APIs and services.
- Validate UI functionality across supported environments.
- QA must verify assigned changes before release.
- Document defects with clear reproduction steps.
- Critical and high-severity defects must be resolved before production deployment.
- Maintain release notes and testing evidence.

</details>

<details>
<summary><b>10 &nbsp;·&nbsp; DevOps & Deployment Standards</b></summary>
<br/>

- Use approved CI/CD workflows.
- Keep deployment configurations version-controlled.
- Separate development, staging and production environments.
- Restrict production deployment permissions.
- Maintain deployment logs and monitoring.
- Define rollback procedures for production releases.
- Do not perform unauthorized infrastructure changes.
- Protect CI/CD credentials and deployment secrets.

</details>

<details>
<summary><b>11 &nbsp;·&nbsp; Documentation Standards</b></summary>
<br/>

| Document | Purpose |
|---|---|
| `README.md` | Project overview and setup |
| `CONTRIBUTING.md` | Contribution guidelines |
| `CHANGELOG.md` | Version and release history |
| `SECURITY.md` | Security reporting policy |
| `LICENSE` | Approved licensing terms |
| API Documentation | API usage and integration details |

Documentation should be clear, accurate and updated alongside code changes.

</details>

<details>
<summary><b>12 &nbsp;·&nbsp; Collaboration & Professional Conduct</b></summary>
<br/>

- Communicate respectfully with all team members.
- Link development work to approved tasks or issues.
- Keep Pull Requests and assigned tasks updated.
- Inform the responsible lead about blockers.
- Share technical knowledge and support team members.
- Respect repository ownership and access permissions.
- Follow company-approved development and release processes.

</details>

<details>
<summary><b>13 &nbsp;·&nbsp; Contribution Workflow</b></summary>
<br/>

1. Get access to the appropriate repository.
2. Review project documentation and coding standards.
3. Create a feature or bug-fix branch.
4. Implement changes following project conventions.
5. Run relevant tests and validations.
6. Commit changes with meaningful messages.
7. Create a Pull Request.
8. Address review feedback.
9. Obtain required approvals.
10. Merge after all required checks pass.

</details>

<p align="center">
  <img src="https://raw.githubusercontent.com/ziuai-ai-tech/.github/main/profile/assets/divider.svg" width="100%" alt=""/>
</p>

<p align="center">
  <i>We believe strong engineering comes from continuous learning, accountability and collaboration.<br/>
  Every team member contributes to building reliable, secure and scalable technology.</i>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ziuai-ai-tech/.github/main/profile/assets/footer.svg" width="100%" alt="Let's build better technology together. Engineering Excellence. Innovation. Reliability."/>
</p>

<p align="center"><sub>ZIUAI &nbsp;·&nbsp; Official GitHub Organization</sub></p>
