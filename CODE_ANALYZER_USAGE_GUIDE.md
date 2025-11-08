# Code Analyzer Agent - Usage Guide

This guide shows you how to use the generic code-analyzer agent to analyze any codebase.

## Quick Start

### Basic Usage

Invoke the agent using the Task tool:

```
Use the code-analyzer agent to analyze this codebase
```

The agent will ask clarifying questions and then provide a comprehensive analysis.

## Usage Patterns

### 1. Comprehensive Analysis

**Use Case**: Get a complete assessment of your entire codebase

```
Use the code-analyzer agent to perform a comprehensive analysis of this codebase
```

**What the agent does:**
- Explores entire project structure
- Analyzes all file types (code, config, docs)
- Assesses quality across all dimensions
- Generates full report with ratings and recommendations

**Best for:**
- New projects you're inheriting
- Pre-production readiness checks
- Quarterly code health reviews
- Due diligence for acquisitions

---

### 2. Focused Analysis by Concern

**Use Case**: Address specific concerns or areas

#### Scalability Focus
```
Use the code-analyzer agent to analyze this codebase for scalability issues
```

**What the agent does:**
- Focuses on architectural patterns
- Identifies bottlenecks and resource constraints
- Assesses horizontal/vertical scalability
- Reviews data processing strategies
- Provides scalability-specific recommendations

**Best for:**
- Planning for growth
- Performance optimization initiatives
- Architecture reviews

#### Security Focus
```
Use the code-analyzer agent to assess security practices in this codebase
```

**What the agent does:**
- Scans for hardcoded credentials
- Reviews authentication/authorization
- Checks input validation
- Assesses secret management
- Identifies security vulnerabilities

**Best for:**
- Security audits
- Pre-deployment reviews
- Compliance requirements

#### Code Quality Focus
```
Use the code-analyzer agent to evaluate code quality and maintainability
```

**What the agent does:**
- Measures code complexity
- Identifies duplication
- Reviews naming conventions
- Assesses documentation
- Checks error handling

**Best for:**
- Code review automation
- Technical debt assessment
- Onboarding new team members

#### Testing Focus
```
Use the code-analyzer agent to analyze testing coverage and quality
```

**What the agent does:**
- Identifies test files and frameworks
- Assesses test coverage
- Reviews test quality and patterns
- Recommends testing improvements

**Best for:**
- QA process improvement
- CI/CD pipeline optimization
- Reducing production bugs

---

### 3. Scoped Analysis by Directory

**Use Case**: Analyze specific parts of the codebase

```
Use the code-analyzer agent to analyze the code in the projects/braintree/p1020_* directories
```

**What the agent does:**
- Limits exploration to specified directories
- Provides focused analysis on that subsystem
- Generates recommendations specific to that scope

**Best for:**
- Module-specific reviews
- Feature branch analysis
- Microservice assessment

---

### 4. Technology-Specific Analysis

**Use Case**: Focus on particular technologies or languages

```
Use the code-analyzer agent to analyze all Python code for best practices
```

```
Use the code-analyzer agent to review SQL query quality and optimization
```

**What the agent does:**
- Filters to specific file types
- Applies language-specific best practices
- Provides technology-specific recommendations

**Best for:**
- Language migration planning
- Framework adoption reviews
- Technology standardization

---

### 5. Quick Assessment

**Use Case**: Rapid overview for time-sensitive decisions

```
Use the code-analyzer agent to provide a quick quality assessment
```

**What the agent does:**
- Samples representative files
- Provides executive summary
- Lists top 3-5 critical issues
- Gives overall rating

**Best for:**
- Triage before deep-dive
- Status updates for stakeholders
- Initial project evaluation

---

### 6. Comparative Analysis

**Use Case**: Compare against standards or benchmarks

```
Use the code-analyzer agent to compare this codebase against data engineering best practices
```

```
Use the code-analyzer agent to benchmark this against industry standards for web applications
```

**What the agent does:**
- Identifies relevant best practices
- Compares current state to standards
- Highlights gaps and strengths
- Provides conformance ratings

**Best for:**
- Process improvement initiatives
- Setting technical standards
- Training and education

---

## Advanced Usage

### Multi-Dimensional Analysis

Request multiple focus areas:

```
Use the code-analyzer agent to analyze scalability, security, and code quality in this codebase
```

### Context-Aware Analysis

Provide context for better recommendations:

```
Use the code-analyzer agent to analyze this ETL pipeline codebase.
We're processing 10M records/day and plan to scale to 100M within 6 months.
Focus on scalability and performance.
```

### Specific File Pattern Analysis

```
Use the code-analyzer agent to analyze all framework modules in projects/framework/**/*.py
```

---

## Interpreting Results

### Understanding Ratings

The agent uses a 5-star rating system for each dimension:

- ⭐⭐⭐⭐⭐ (9-10/10): Excellent - Industry leading
- ⭐⭐⭐⭐ (7-8/10): Good - Meets best practices
- ⭐⭐⭐ (5-6/10): Acceptable - Room for improvement
- ⭐⭐ (3-4/10): Needs Work - Significant issues
- ⭐ (1-2/10): Poor - Critical problems

### Recommendation Priorities

**Priority 1 - Critical**: Address immediately (within current sprint)
- Usually high impact, low-to-medium effort
- Often security or critical functionality issues

**Priority 2 - High**: Address soon (within 1-2 months)
- High impact on quality or performance
- Moderate effort required

**Priority 3 - Medium**: Address when possible (within quarter)
- Moderate impact
- Can be scheduled in backlog

**Priority 4 - Low**: Nice to have (future consideration)
- Low impact or very high effort
- Long-term improvements

### Effort Estimates

- **Low**: Hours to 1-2 days
- **Medium**: 3-7 days
- **High**: 1-4 weeks
- **Very High**: Months (architectural changes)

---

## Example Workflows

### Workflow 1: Pre-Production Checklist

1. **Run comprehensive analysis**
   ```
   Use the code-analyzer agent to perform comprehensive analysis
   ```

2. **Review Priority 1 and 2 recommendations**

3. **Address critical issues before deployment**

4. **Plan Priority 3 and 4 for future sprints**

### Workflow 2: Technical Debt Reduction

1. **Focus on code quality**
   ```
   Use the code-analyzer agent to evaluate code quality and identify technical debt
   ```

2. **Identify duplication hotspots**

3. **Create refactoring plan based on recommendations**

4. **Track progress with follow-up analysis**
   ```
   Use the code-analyzer agent to compare current code quality against previous analysis
   ```

### Workflow 3: Scaling Preparation

1. **Analyze scalability**
   ```
   Use the code-analyzer agent to assess scalability for 10x growth
   ```

2. **Identify bottlenecks**

3. **Implement high-priority improvements**

4. **Load test and validate**

5. **Re-analyze for remaining issues**

### Workflow 4: Code Review Automation

1. **Analyze feature branch**
   ```
   Use the code-analyzer agent to analyze code in feature/new-payment-gateway
   ```

2. **Review recommendations in PR comments**

3. **Address issues before merging**

4. **Use as checklist for manual review**

---

## Tips for Best Results

### 1. Be Specific About Your Goals

❌ **Vague**: "Analyze this code"
✅ **Specific**: "Analyze this ETL pipeline for performance bottlenecks handling 50M daily records"

### 2. Provide Context

Include relevant information:
- Project type (ETL, web app, API, library)
- Scale (users, data volume, transactions/sec)
- Technology stack (if known)
- Specific concerns or incidents
- Timeline constraints

### 3. Start Broad, Then Focus

1. First run: Comprehensive analysis
2. Second run: Deep-dive on specific issues found
3. Third run: Verify improvements

### 4. Use for Different Project Types

The agent adapts to:
- **ETL/Data Pipelines**: Focuses on incremental loads, data quality, scalability
- **Web Applications**: Focuses on MVC, REST APIs, security, performance
- **Microservices**: Focuses on service boundaries, inter-service communication, resilience
- **Libraries/Packages**: Focuses on API design, documentation, backward compatibility
- **Data Science Projects**: Focuses on reproducibility, model management, data versioning

### 5. Iterative Improvement

Use the agent regularly:
- Before major releases
- After implementing recommendations
- When adopting new technologies
- During architecture reviews
- For onboarding documentation

---

## Common Use Cases

### For Individual Developers

```
Use the code-analyzer agent to review my recent changes in src/payment-processor/
```

- Pre-commit quality checks
- Learning best practices
- Code improvement ideas

### For Team Leads

```
Use the code-analyzer agent to assess technical debt across our codebase
```

- Sprint planning input
- Technical roadmap creation
- Team skill gap identification

### For Architects

```
Use the code-analyzer agent to evaluate architectural patterns and scalability
```

- Architecture decision validation
- Technology selection support
- Migration planning

### For Product Managers

```
Use the code-analyzer agent for a quick executive summary of code health
```

- Risk assessment
- Release readiness
- Resource planning

### For DevOps/SRE

```
Use the code-analyzer agent to analyze deployment, monitoring, and error handling
```

- Reliability improvements
- Incident post-mortem analysis
- SLA optimization

---

## Customization Options

When invoking the agent, you can specify:

### Depth Level
- **Quick**: "provide a quick assessment"
- **Standard**: (default, no modifier needed)
- **Comprehensive**: "perform a comprehensive analysis"

### Output Format
- **Executive Summary**: "provide an executive summary"
- **Detailed Report**: (default)
- **Action Plan**: "create an actionable improvement plan"

### Focus Areas
- Single: "focus on security"
- Multiple: "focus on scalability and performance"
- All: "analyze all dimensions"

---

## Integration with Development Workflow

### Git Hooks (Pre-commit)
```bash
# .git/hooks/pre-commit
Use the code-analyzer agent to analyze staged changes
```

### CI/CD Pipeline
```yaml
# .github/workflows/code-analysis.yml
- name: Code Quality Analysis
  run: |
    Use the code-analyzer agent to analyze this codebase
```

### Regular Reviews
- Weekly: Quick assessment of changes
- Monthly: Comprehensive analysis
- Quarterly: Benchmark against industry standards

---

## Troubleshooting

### Agent asks too many questions
→ Provide more context in your initial request

### Analysis is too shallow
→ Request "comprehensive" or "deep-dive" analysis
→ Specify the depth level you need

### Analysis is too broad
→ Specify directory scope
→ Focus on specific technologies
→ Limit to particular concerns

### Want specific code examples
→ Ask: "show me code examples of the duplication issues"
→ Request: "provide before/after code samples"

---

## FAQ

**Q: How long does analysis take?**
A: Depends on codebase size and depth:
- Quick: 2-5 minutes
- Standard: 5-15 minutes
- Comprehensive: 15-45 minutes

**Q: Can I analyze just changed files?**
A: Yes! Specify the scope:
```
Use the code-analyzer agent to analyze files modified in the last commit
```

**Q: Does it work with any programming language?**
A: Yes, the agent is language-agnostic and adapts to:
- Python, Java, JavaScript/TypeScript, Go, Ruby, PHP, C#, etc.
- SQL dialects (PostgreSQL, MySQL, BigQuery, etc.)
- Configuration languages (YAML, JSON, TOML, etc.)

**Q: Can it detect security vulnerabilities?**
A: It identifies common security issues like:
- Hardcoded credentials
- SQL injection patterns
- Missing input validation
- Insecure configurations

For deep security scanning, use specialized tools like Snyk, SonarQube, or Bandit.

**Q: How accurate are the recommendations?**
A: Recommendations are based on:
- Industry best practices
- Language-specific standards (PEP 8, ESLint, etc.)
- Common design patterns
- Actual code analysis

Always apply professional judgment and consider your specific context.

**Q: Can I use this for non-code files?**
A: Yes! The agent can analyze:
- Documentation (README, wikis)
- Configuration files
- Infrastructure as Code (Terraform, CloudFormation)
- CI/CD pipelines
- Database schemas

---

## Next Steps

1. **Try it now** with a simple request:
   ```
   Use the code-analyzer agent to provide a quick assessment of this codebase
   ```

2. **Review the results** and identify top priorities

3. **Create action items** from recommendations

4. **Re-run analysis** after improvements to track progress

5. **Share insights** with your team

---

## Support and Feedback

- For issues with the agent, check the agent definition at `.claude/agents/code-analyzer.md`
- To customize the agent, edit the markdown file
- To add new analysis dimensions, extend the agent prompts
- To share improvements, document them in your team wiki

---

**Remember**: The code analyzer is a tool to support your judgment, not replace it. Use the insights as a starting point for discussions and improvements, always considering your specific context, constraints, and goals.
