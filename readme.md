https://github.com/wahyudialfurqon/PM-Lecture-S23/releases

[![Releases](https://img.shields.io/badge/Releases-Download-blue?logo=github&style=for-the-badge)](https://github.com/wahyudialfurqon/PM-Lecture-S23/releases)

Programmiermethoden S23 — Clean Code, Java, Testing, Git

[![Course Topics](https://img.shields.io/badge/Topics-clean--code%20%7C%20git%20%7C%20java%20%7C%20testing-orange?style=for-the-badge)](https://github.com/wahyudialfurqon/PM-Lecture-S23)
[![OER](https://img.shields.io/badge/OER-open--educational--resources-green?style=for-the-badge)](https://github.com/wahyudialfurqon/PM-Lecture-S23)
![Hacktoberfest](https://img.shields.io/badge/Hacktoberfest-welcome-purple?style=for-the-badge)

![Java Logo](https://upload.wikimedia.org/wikipedia/en/3/30/Java_programming_language_logo.svg) ![Git Logo](https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png) ![Testing Icon](https://upload.wikimedia.org/wikipedia/commons/6/6a/OOjs_UI_icon_check.svg)

Table of Contents
- Course overview
- How to use this repository
- Releases (download and execute)
- Syllabus and lecture map
- Lecture notes and slides
- Lab exercises and solutions
- Assignments and grading
- Code style and clean code rules
- Refactoring patterns
- Testing strategy and examples
- Logging and observability
- Git workflow and best practices
- Teaching materials and OER policy
- Contribution guide
- Build and run
- CI, tests, and badges
- FAQ
- Maintainers and contact

Course overview
This repository holds material for the course "Programmiermethoden" (Summer 2023). The material targets undergraduate students and developers who want to improve code quality. The course covers core practices: clean code, refactoring, testing, logging, Git, and practical Java. It mixes theory and lab work. It focuses on hands-on tasks and clear code.

How to use this repository
- Clone the repo to your machine.
- Read the syllabus to plan your study.
- Open the lecture notes for each week.
- Run the labs in the lab folder.
- Use the tests to verify your code.
- Submit work via the steps in the Assignments section.

Quick clone
git clone https://github.com/wahyudialfurqon/PM-Lecture-S23.git

Releases (download and execute)
The official release page lists packaged materials, slides, and runnable demos. Download the release asset that matches your platform and run it.

Release link:
https://github.com/wahyudialfurqon/PM-Lecture-S23/releases

What to do
- Visit the link above.
- Download the release file for the demo you want.
- Execute the file after download.

Common run commands
- JAR (Java demo)
  - Unix: java -jar pm-lecture-demo-VERSION.jar
  - Windows: java -jar pm-lecture-demo-VERSION.jar
- ZIP (slides and notes)
  - Unix: unzip pm-lecture-slides-VERSION.zip -d pm-slides
  - Windows: Expand-Archive -Path pm-lecture-slides-VERSION.zip -DestinationPath .\pm-slides
- Shell script (tools)
  - Unix: chmod +x pm-tools-VERSION.sh && ./pm-tools-VERSION.sh

If a release link changes or the asset does not open, check the Releases section on the project page. Use the releases page as the single source for downloadable artifacts.

Syllabus and lecture map
This section lists topics by week. Each week links to slides, examples, and labs.

Week 1 — Foundations
- Course goals and assessment.
- Java toolchain and project layout.
- Clean code basics: naming, small functions, single responsibility.
- Lab 1: Setup and simple refactor.

Week 2 — Git and version control
- Commit design.
- Branch models and merge strategies.
- Rebase vs merge.
- Pull requests and code review.
- Lab 2: Branching and feature workflow.

Week 3 — Unit testing
- JUnit basics.
- Test-driven development (TDD) patterns.
- Mocking and dependency injection.
- Lab 3: Write tests first for a small module.

Week 4 — Refactoring I
- Code smells and detection.
- Small refactor steps.
- Automated refactor tools in IDE.
- Lab 4: Refactor legacy code to improve readability.

Week 5 — Refactoring II
- Extract method, inline method, move method.
- Replace conditional with polymorphism.
- Performance-aware refactor.
- Lab 5: Apply design changes with tests.

Week 6 — Logging and debugging
- Logging levels and layout.
- Structured logging.
- How to trace runtime issues with logs.
- Lab 6: Add logging to a service and use it to debug.

Week 7 — Integration testing and CI
- Integration tests vs unit tests.
- Using Docker for integration tests.
- CI pipelines that run tests and build artifacts.
- Lab 7: Add a CI job to build and test.

Week 8 — Design patterns and clean architecture
- Common patterns: factory, strategy, observer.
- Layered architecture and boundaries.
- How patterns help refactor and test.
- Lab 8: Implement a small plugin using strategy.

Week 9 — Test doubles and property testing
- Stubs, mocks, spies.
- Property-based testing basics.
- Test coverage vs test quality.
- Lab 9: Convert example tests to use property testing.

Week 10 — Performance and profiling
- CPU and memory profiling.
- Common performance anti-patterns.
- Tools: VisualVM, Java Flight Recorder.
- Lab 10: Profile an app and fix hot paths.

Week 11 — Code quality metrics and static analysis
- Linters and static analyzers.
- SonarQube basics.
- How to integrate checks into CI.
- Lab 11: Run static checks and fix violations.

Week 12 — Final labs and project presentations
- Project showcase.
- Peer review and code review checklist.
- Course retro.

Lecture notes and slides
Each lecture folder contains:
- PDF slides.
- Markdown notes with code snippets.
- Example projects.
- Suggested reading.

Folder layout
- docs/lectures/week-01
  - slides.pdf
  - notes.md
  - examples/
- docs/lectures/week-02
  - slides.pdf
  - notes.md
  - examples/

How to view slides
- Download the release that contains slides or open the slides in the docs folder.
- Use any PDF viewer or your browser.

Lab exercises and solutions
Labs follow the test-first approach. Each lab has:
- Problem statement.
- Starter code.
- Tests that must pass.
- Solution branch for instructors.

Lab example structure
- labs/lab-01/
  - README.md
  - src/
  - test/
  - build.gradle or pom.xml

How to run a lab
- Build the project.
- Run the tests.
- Implement the code until tests pass.

Example commands
- Gradle
  - ./gradlew test
  - ./gradlew run
- Maven
  - mvn test
  - mvn -DskipTests=false verify

Assignments and grading
Assignments vary by year. The structure below reflects the S23 plan.

Assignment types
- Small exercises (individual). Low weight.
- Labs (individual). Medium weight.
- Projects (group). High weight.
- Quizzes (online). Low weight.

Assessment criteria
- Correctness: tests pass.
- Code quality: clarity, style, and design.
- Tests: coverage and meaningful test cases.
- Documentation: README and comments.
- Git history: meaningful commits and branch usage.

Submission process
- Create a fork.
- Implement work on a feature branch.
- Push commits to your fork.
- Open a pull request against the course repo or submit via the learning platform.
- Use clear PR descriptions and link issues.

Grading rubric (example)
- Tests and correctness: 50%
- Code quality and refactor: 20%
- Documentation and README: 15%
- Git workflow and commits: 10%
- Presentation and demo: 5%

Code style and clean code rules
Follow a strict yet practical code style. The style improves readability and reduces defects.

Naming
- Use precise names.
- Use verbs for methods that perform actions.
- Use nouns for classes and modules.

Functions
- Keep functions short.
- One responsibility per function.
- Limit parameters to three when possible.

Classes
- Keep classes focused.
- Prefer composition over inheritance when needed.
- Use interfaces for boundary points.

Formatting and layout
- Use consistent indentation.
- Keep line length under 100 characters.
- Group related code and tests.

Comments and documentation
- Use comments to explain why, not what.
- Prefer self-explanatory code over comments.
- Write README for modules that need explanation.

Clean code checklist
- Does the class name match its responsibility?
- Does the method name match its action?
- Can I read the code without heavy mental work?
- Are edge cases tested?

Refactoring patterns
Refactor with small steps. Use tests to ensure behavior stays the same.

Common refactor patterns
- Extract Method: pull code into a new method with a clear name.
- Inline Method: replace trivial method calls with the body.
- Rename: give clear names to variables and functions.
- Move: relocate method or field to a better class.
- Replace Conditional with Polymorphism: use subclasses or strategy.
- Replace Magic Number with Named Constant.

Refactor workflow
- Run tests.
- Make a small change.
- Re-run tests.
- Commit the change.
- Repeat.

Refactor example
Start with a long method. Extract parts to methods with meaningful names. Each extraction creates a testable unit.

Testing strategy and examples
Testing forms the core quality gate. Tests act as documentation and safety net.

Test pyramid
- Unit tests: fast and isolated. Many.
- Integration tests: test component interaction. Fewer.
- End-to-end tests: cover user flows. Few.

Unit testing best practices
- Test one behavior per test.
- Use descriptive test names.
- Mock external dependencies.
- Keep tests deterministic.
- Prefer in-memory fixtures for speed.

Example unit test (JUnit 5)
- Use @Test for test methods.
- Use @BeforeEach to set up.
- Use assertions from assertj or JUnit.

Mocking
- Use Mockito for method stubbing and verification.
- Avoid heavy mocking of internal logic.
- Test behavior, not implementation.

Property-based testing
- Use libraries like jqwik or junit-quickcheck.
- Define properties instead of fixed cases.
- Good to find edge cases.

Testing anti-patterns
- Tests that check private implementation.
- Overuse of sleeps or waits.
- Tests that depend on timing.

Logging and observability
Logs help track runtime behavior. Use logging as a first aid when debugging.

Logging levels
- TRACE: detailed, low-level events.
- DEBUG: diagnostic information.
- INFO: runtime facts that matter.
- WARN: recoverable issues.
- ERROR: unrecoverable errors.

Structured logging
- Use key-value pairs.
- Make logs parseable by tools.
- Keep context in MDC (Mapped Diagnostic Context).

Log examples
- Bad: logger.debug("User id: " + id);
- Good: logger.debug("user.login attempt", kv("userId", id));

Debugging with logs
- Add context early.
- Keep logs short but informative.
- Rotate logs and set retention.

Logging framework
- Use SLF4J as facade.
- Use Logback or Log4J2 as backend.

Git workflow and best practices
Use Git to maintain a clear project history. Use branches for features and fixes.

Branch model
- main (or master) for stable releases.
- develop for integration.
- feature/* for new work.
- fix/* for hotfixes.

Commits
- Write clear commit messages.
- Use imperative present tense: "Add user validation".
- Limit a commit to one logical change.

Pull requests
- Open PRs early.
- Describe the intent and scope.
- Link to issues.
- Run CI and fix failing checks.

Rebase vs merge
- Rebase to keep a linear history.
- Use merge for public branches to preserve history.

Example git commands
- Start feature: git checkout -b feature/new-parser
- Stage: git add .
- Commit: git commit -m "Implement basic parser"
- Rebase: git fetch && git rebase origin/main
- Push: git push -u origin feature/new-parser
- Open PR.

Teaching materials and OER policy
The course uses open educational resources (OER). Materials may reuse permissive content and follow open licenses.

What this repo provides
- Slides under a permissive license.
- Lab code with a license file.
- Examples for teaching and reuse.

Reuse rules
- Keep attribution intact as required by the license.
- Follow the license when remixing the content.

Images and media
We include images from public sources and own materials. When reusing images, check license.

Contribution guide
Contributions improve the course and broaden access. The repo welcomes edits to slides, tests, and labs.

How to contribute
- Fork the repo.
- Create a branch for your change.
- Run tests locally.
- Create a pull request with a clear description.
- Add tests for new behavior.

Good contribution practices
- Keep PRs small and focused.
- Add tests for every behavior change.
- Respect the existing code style.
- Keep documentation up to date.

Issue types
- Bug reports: reproducible steps and logs.
- Feature requests: clear goal and use case.
- Typos and doc fixes: small PRs accepted.

Labeling
- good-first-issue: suitable for new contributors.
- help-wanted: maintainers welcome assistance.
- hacktoberfest: issues that qualify.

Build and run
The project uses standard Java build tools. Use Gradle or Maven based on the sample.

Prerequisites
- JDK 11 or later.
- Git.
- Gradle or Maven.

Common commands
- Build: ./gradlew build or mvn clean package
- Test: ./gradlew test or mvn test
- Run: java -jar build/libs/pm-lecture-demo.jar

Docker support
- The repo includes Dockerfile for demos.
- Build image: docker build -t pm-demo:latest .
- Run: docker run -p 8080:8080 pm-demo:latest

CI, tests, and badges
The repo integrates CI to run tests and checks. Badges show the current status.

Common CI steps
- Check out code.
- Set up JDK.
- Build and run tests.
- Run static analyzers.
- Publish artifacts to releases on tag.

Badges
- Build status
- Code coverage
- Latest release

FAQ
Q: How do I run a lab?
A: Build the project and run the test suite. Implement the code until tests pass.

Q: Where are the slides?
A: Slides are in docs/lectures and in the release archive.

Q: How do I get a copy of the demo app?
A: Download the demo file from the Releases page and execute it.

Q: What Java version do I need?
A: Use JDK 11 or newer.

Typical troubleshooting
- Tests fail on a new machine: run a clean build and check mem limits.
- CI fails with formatting: run the formatter locally.
- Merge conflicts: rebase and resolve conflicts, then push.

Resources and reading list
This section lists recommended books and articles linked to topics from the course.

Books
- "Clean Code" by Robert C. Martin
- "Refactoring" by Martin Fowler
- "Working Effectively with Legacy Code" by Michael Feathers
- "Test Driven Development" by Kent Beck

Articles
- Blog posts on code smells.
- Git workflow guides.
- JUnit and Mockito docs.

Tools and plugins
- IDE: IntelliJ IDEA or VS Code with Java extensions.
- Build: Gradle or Maven.
- Static analysis: SpotBugs, PMD, Checkstyle.
- Logging: SLF4J, Logback.
- Test: JUnit 5, Mockito, AssertJ.

Example projects in repo
- parser-demo: shows parsing and tests.
- logger-demo: shows logging best practices.
- refactor-demo: before and after refactor samples.

Teaching notes for instructors
Instructors can reuse slides and labs. Each lab contains expected student outcomes and sample solutions.

Session plan
- Presentation: 30–40 minutes.
- Live coding: 20 minutes.
- Lab time: 30–40 minutes.
- Q&A and wrap up: 10 minutes.

Assessment tips
- Calibrate grading by checking a subset of submissions.
- Use tests to automate correctness checks.
- Run manual code review for design feedback.

License
This project uses an open license. See LICENSE.md in the repo root. The license permits teaching reuse and derivative work with attribution.

Code of conduct
Contributors must follow community standards. Be respectful and constructive. Report issues to maintainers.

Repository layout
- README.md
- docs/
  - lectures/
  - labs/
- examples/
- src/
- test/
- .github/
  - workflows/
  - CONTRIBUTING.md
- LICENSE.md

Examples and snippets
Small examples help in class.

Refactor example (pseudocode)
Before:
class OrderProcessor {
  void process(Order o) {
    if (o.type == "X") { // ...
    } else if (o.type == "Y") { // ...
    }
  }
}

After:
interface OrderHandler { void handle(Order o); }
class XOrderHandler implements OrderHandler { /*...*/ }
class YOrderHandler implements OrderHandler { /*...*/ }
class OrderProcessor {
  Map<String, OrderHandler> handlers;
  void process(Order o) { handlers.get(o.type).handle(o); }
}

Testing example
@Test
void calculateTotal_returnsCorrectSum() {
  Cart cart = new Cart();
  cart.add(new Item("A", 10));
  cart.add(new Item("B", 15));
  assertThat(cart.total()).isEqualTo(25);
}

Logging example
logger.info("order.process start", kv("orderId", id));

Maintainers and contact
- Course lead: Dr. Example Name — email maintained in repo.
- TAs: see CONTRIBUTORS.md

Community channels
- GitHub issues
- Course forum or learning platform
- Office hours schedule in docs

Accessibility and formats
Slides come as PDF and HTML. Labs include machine-readable tests and plain text descriptions.

Localization
Materials contain German and English notes. Contributors can add translations in docs/i18n/.

Quality gates
- All PRs must pass CI.
- Tests must run under Gradle or Maven.
- New code needs unit tests.

Sample contribution flow
1. Fork the repo.
2. Create branch feature/topic-fix.
3. Implement change and add tests.
4. Run ./gradlew test and static checks.
5. Push branch.
6. Open PR and request review.

Releases and artifacts
Releases publish packaged slides, demo jars, and lab starter kits. Download and execute the appropriate file.

Release link (again for quick access):
https://github.com/wahyudialfurqon/PM-Lecture-S23/releases

Release usage reminder
- Pick the asset for your platform.
- Download the file.
- Execute the file as shown in the commands above.

Security and dependencies
- Keep dependencies up to date.
- Use CVE scans in CI.
- Avoid pulling untrusted binaries.

Appendix A — Lab checklist
- Read the lab README.
- Run the test suite.
- Implement smallest failing part.
- Commit often with clear messages.
- Open PR or submit via the platform.

Appendix B — Code review checklist
- Does this change have tests?
- Do names convey intent?
- Is behavior unchanged where refactor occurred?
- Is the commit history clear?
- Is the change small and focused?

Appendix C — Sample rubric for project
- Functionality: 50 points
- Code quality: 20 points
- Tests: 20 points
- Documentation: 10 points

Images and media credits
- Java logo: Wikipedia
- Git logo: git-scm.com
- Check icon: Wikimedia commons

End of file