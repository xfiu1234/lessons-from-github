# lessons-from-github
A compilation of professional principles and lessons learned from nearly a decade defending the internet from baddies at GitHub

## About This Content

- This repository contains principles and lessons learned from the author's real work experiences, materials, and personal notes from more than nine years at GitHub, compiled with assistance from AI.
- The content includes nothing sensitive or confidential, nor any intellectual property from GitHub. Some examples may be modified or partially contrived to convey context and preserve confidentiality.
- The advice and perspectives shared here are solely those of the author and should not be considered official recommendations or positions of GitHub.
- As this content was compiled with the assistance of AI, it is presently somewhat lengthy and repetitive.  It is subject to further revision by the author.

This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

---

## Key Lessons from 9+ Years of Growing Up with GitHub Security
**Practical Guidance for Security and Engineering Professionals**

---

### Table of Contents
- [Leadership & Culture](#leadership--culture)
- [Strategic Thinking & Execution](#strategic-thinking--execution)
- [Risk Management & Business Alignment](#risk-management--business-alignment)
- [Crisis Management](#crisis-management)
- [Communication & Influence](#communication--influence)
- [Coalition Building & Cross-functional Work](#coalition-building--cross-functional-work)
- [Process & Governance](#process--governance)
- [Career Development](#career-development)
- [Security-Specific Lessons](#security-specific-lessons)
- [Engineering Principles](#engineering-principles)
- [Legacy Building](#legacy-building)
- [Core Planning & Strategy Principles](#core-planning--strategy-principles)

---

### Leadership & Culture

#### 1. Model Empathetic and Inclusive Leadership

**Core Principle:**
> **Leadership isn't about authority—it's about empowerment.** The most effective leaders create environments where others can succeed, especially during crises when stress is highest.

**Practical Application:**
- During incidents, focus on clarity and support, not blame
- Make time for mentoring even when you're busy
- Model the behavior you want to see in your organization
- Lead with questions, not just answers
- Practice blameless post-mortems that focus on learning

**Key Insight:**
Leadership through empowerment means creating conditions where others can take ownership and succeed, rather than centralizing control. This builds organizational resilience and scales impact beyond individual contributions.

#### 2. Scale Impact Through Empowerment, Not Execution

**Core Principle:**
> **As you advance, your impact scales through others, not just through your own execution.** The transition from "doing" to "enabling" is critical for senior IC and management roles. The most scalable leadership model is one where you become increasingly unnecessary for day-to-day execution.

**Practical Application:**
- Identify opportunities to teach rather than just complete tasks
- Build coalitions and empower DRIs on strategic initiatives
- Share credit broadly and create opportunities for others
- Focus on system design and architecture, not just implementation
- **Clearly identify Directly Responsible Individuals (DRIs)** for initiatives and ensure they have the authority and resources to succeed
- Document processes and decision-making frameworks
- Create "bus factor" resilience (what happens if you're unavailable?)
- Resist the urge to be the hero on every project
- **Establish governance**: Participate in or help establish steering committees, working groups to track progress and ensure accountability

**Career Indicator:**
When you find yourself being the critical path for too many initiatives, it's time to shift to empowerment mode.

**Success Metric:**
Projects should continue successfully after you transition off them. If everything falls apart when you leave, you haven't built sustainability.

**Staff+ Perspective:**
Advancing into Staff Engineer roles requires demonstrating that you can drive impact through influence, architecture, and enabling others—not just through personal execution. Practice delegating execution while maintaining strategic oversight.

#### 3. Stay Calm Under Pressure

**Core Principle:**
> **Your team takes their emotional cues from you during a crisis.** Panic spreads; calm is contagious. Clear-headed leadership in chaos is a learnable skill.

**Practical Application:**
- Practice incident response in non-crisis situations (game days, tabletops)
- Develop a personal checklist for crisis situations
- Focus on what you can control and influence
- Use clear, direct language; avoid speculation
- Take breaks during long incidents to maintain clarity

**Red Flag:**
If you find yourself becoming the source of stress during incidents rather than a stabilizing force, take some time off to recharge and fend off burnout, work to improve emotional regulation skills, or consider whether it's time to move out of incident/crisis roles.

### Strategic Thinking & Execution

#### 4. Identify Systemic Problems, Not Just Symptoms

**Core Principle:**
> **The best security and engineering work prevents entire classes of problems, not just individual incidents.** Look for patterns across incidents and design systemic solutions.

**Practical Application:**
- After each incident, ask "How could this entire class of problems be prevented?"
- Track recurring themes across multiple incidents or issues
- Invest time in root cause analysis beyond immediate fixes
- Think in terms of architecture and systems, not just point solutions
- **Use risk assessment as a tool to influence roadmaps and priorities** by identifying high-impact, high-likelihood risks

**Example Pattern:**
- **Symptom**: Multiple internal credential exposure incidents
- **Root Cause**: No systematic detection or prevention
- **Systemic Solution**: Secret scanning, developer education, zero secrets goal
- **Result**: Entire vulnerability class eliminated

**Risk-First Approach:**
Pattern recognition should lead to risk assessment: What are the potential architectural, operational, or security risks that could impact multiple teams? Quantify the business impact (not just technical severity) to prioritize systemic solutions appropriately.

#### 5. Multi-Year Strategic Thinking

**Core Principle:**
> **Transformational change takes years, not quarters.** Be willing to commit to multi-year strategic initiatives with measurable milestones along the way.

**Practical Application:**
- Think in 2-3 year horizons for strategic work
- Break long-term goals into quarterly/half-yearly milestones
- Communicate progress regularly to maintain organizational commitment
- Build sustainability into the plan (don't burn yourself or the team out)
- Accept that some initiatives will outlast your direct involvement
- **Define SMART objectives** (Specific, Measurable, Achievable, Relevant, Time-bound) to provide clear direction

**Reality Check:**
If you're only working on things that can be completed in a single quarter, you're probably not working at a strategic level.

**Strategic Alignment Principle:**
Ensure technical and security initiatives are clearly tied to broader organizational goals and business outcomes. Develop the ability to articulate how specific technical projects directly contribute to strategic goals or solve business problems.

#### 6. Balance Strategic Vision with Tactical Execution

**Core Principle:**
> **Strategic leaders who've lost touch with tactical reality make poor decisions.** Stay connected to the execution layer even as you move to strategy roles.

**Practical Application:**
- Participate in oncall rotations even in senior roles (when appropriate)
- Review incident post-mortems regularly
- Spend time with teams executing your strategic initiatives
- Test your own strategic recommendations with real implementation work
- Stay technically credible by keeping hands-on skills current
- **Use data and metrics to ground strategic decisions** in operational reality

**Bias for Action:**
Strategic thinking doesn't mean slow planning. Emphasize moving quickly, making timely decisions, and driving execution while maintaining strategic alignment. Break down large initiatives into actionable phases and push for progress.

#### 7. Design Sustainable Systems That Scale Without Heroes

**Core Principle:**
> **One-time fixes create technical debt; sustainable solutions build organizational capability.** Design systems, processes, and initiatives that continue to deliver value long after initial implementation. If your process depends on heroic effort or specific individuals, it will fail under scale or turnover.

**Practical Application:**
- Ask "What happens to this in 2 years?" during design
- Build processes that scale with team/company growth
- Create documentation and training for sustainability
- Design for operator succession (what if the expert leaves?)
- Avoid solutions that require heroic ongoing effort
- **Aim to "level up" capabilities rather than applying temporary fixes**
- Focus on preventing "risk relapse" by building durable solutions
- Document processes clearly (runbooks, playbooks, checklists)
- Distribute knowledge and ownership across team members
- Build escalation paths and backup coverage
- Test processes with new team members
- Automate repetitive tasks
- Design for growth and turnover

**Sustainability Test:**
Can a new team member execute this process with documentation alone? Does the process scale linearly with growth, or sub-linearly? What happens if the primary owner is unavailable for 2 weeks? 2 months? Is tribal knowledge documented or still in people's heads?

**Architectural Perspective:**
Champion architectural patterns and practices that support scalability, reliability, security, and ease of maintenance. Address technical debt strategically as part of long-term initiatives, not as separate cleanup work.

### Risk Management & Business Alignment

#### 8. Embrace a Risk-First Perspective

**Core Principle:**
> **Risk management isn't just about preventing incidents—it's about enabling business outcomes by addressing what could prevent success.** The best technical leaders think in terms of business impact, not just technical severity.

**Practical Application:**
- **Identify and articulate systemic risks** that could impact multiple teams or the entire organization
- **Quantify risk impact** in business terms: revenue impact, customer trust, future velocity, market position
- **Drive risk-informed prioritization** using risk assessment to influence roadmaps at the appropriate organizational level
- Make risk trade-offs explicit in planning documents
- Connect risk mitigation work to business objectives
- Communicate risks proactively to relevant stakeholders

**Risk Assessment Framework:**
1. **Identify**: What could go wrong? (technical, operational, security, compliance)
2. **Analyze**: What's the likelihood and business impact?
3. **Prioritize**: Which risks warrant immediate attention vs. monitoring?
4. **Mitigate**: What systemic solutions address root causes?
5. **Monitor**: How do we know if risk posture is improving?

**For Aspiring Staff Engineers:**
Go beyond project-level risks. Learn to identify architectural, operational, and security risks that span organizational boundaries. Develop the ability to explain technical risks in business terms that executives can act upon.

#### 9. Champion Strategic Alignment and Position Work as Business Enabler

**Core Principle:**
> **Technical excellence without business alignment is just expensive hobby work.** The most impactful technical leaders ensure their work directly supports organizational strategy and business outcomes. Security that blocks business doesn't survive long-term—frame initiatives in terms of business value, customer trust, and competitive advantage.

**Practical Application:**
- **Understand the "Why"**: Develop deep understanding of company's business strategy, product roadmap, and key results (OKRs)
- **Trace technical work to business outcomes**: Practice articulating how specific projects directly contribute to strategic goals
- **Proactively identify alignment opportunities**: Look for ways technology can enable new business opportunities
- Frame security requirements as customer expectations and competitive advantages
- Connect infrastructure investments to future business capabilities
- Position technical initiatives in terms of business value: revenue enablement, customer trust, market differentiation, operational efficiency
- Lead with business outcomes, not security jargon
- Build security into the development process, not as a gate
- Measure success by business metrics, not just security metrics
- **Consider customer and ecosystem impact**: Evaluate how decisions affect user experience, reliability, and broader ecosystem

**Strategic Alignment Checklist:**
- Does this initiative support a specific business objective or OKR?
- Can I explain the business value in terms executives understand?
- How does this enable future business capabilities or remove constraints?
- What's the customer/user impact of this work?
- If we don't do this, what business outcomes are at risk?

**Reframing Examples:**
- ❌ "We need better logging infrastructure"
- ✅ "Investing in logging enables faster incident response, reducing customer impact and supporting our reliability commitments"

- ❌ "Technical debt is slowing us down"
- ✅ "Addressing technical debt in [area] will increase feature delivery velocity by X%, enabling faster response to market opportunities"

- ❌ "We need 2FA to reduce account takeover risk"
- ✅ "2FA will strengthen trust in the software supply chain and differentiate us in the market"

#### 10. Define Clear, Measurable Objectives

**Core Principle:**
> **If you can't measure it, you can't manage it—and you can't prove you succeeded.** SMART objectives provide clarity, enable tracking, and demonstrate impact.

**Practical Application:**
- **Set ambitious, outcome-oriented goals** focused on desired *impact* (reduce recovery time by X%, improve reliability to Y nines) not outputs (build feature Z)
- **Establish key metrics** before starting: What data demonstrates success?
- **Define success criteria**: What does "done" look like? What's "good enough"?
- **Communicate objectives compellingly**: Ensure stakeholders understand goals, importance, and how their work contributes
- Break long-term objectives into measurable milestones
- Track and report progress regularly

**SMART Objectives Framework:**
- **Specific**: Precisely defined outcome
- **Measurable**: Quantifiable success criteria
- **Achievable**: Realistic given resources and constraints
- **Relevant**: Aligned with business goals
- **Time-bound**: Clear deadline or timeframe

**Examples:**
- "Deliver 2FA requirements to X million users by Q1 2024 with >90% adoption"
- "Achieve zero secrets in source code by Q4"
- "Maintain <1 hour MTTD for SEV-0/1 incidents"

### Crisis Management

#### 11. Lead Complex Crises with Clear Communication

**Core Principle:**
> **Crisis leadership is about coordination, not heroics.** The leader's job is to create clarity, align stakeholders, make decisions with incomplete information, and maintain forward momentum. In a crisis, clarity beats completeness—tell people what they need to know and what they need to do, quickly and unambiguously.

**Practical Application:**
- Establish clear incident command structure before crises occur
- Create decision-making frameworks for time-sensitive situations
- Practice coordinating across many teams (not just technical teams)
- Develop templates/checklists for different crisis types
- Build relationships before you need them in a crisis
- **Cultivate bias for action**: Move quickly, make timely decisions, drive execution
- Lead with the TL;DR (what happened, what's the impact, what action is needed)
- Use clear, direct language; avoid jargon when possible
- Provide specific next steps, not vague guidance
- Update regularly, even if "no new information" is the update
- Separate facts from speculation/analysis
- Use formatting (bold, bullets, headers) to improve scannability

**Key Skills:**
1. **Rapid assessment**: Quickly understand scope and impact
2. **Clear communication**: Regular updates to stakeholders at appropriate levels
3. **Decisive action**: Make calls with incomplete information
4. **Coordination**: Keep multiple workstreams aligned
5. **Post-crisis learning**: Convert crisis to organizational improvement

**Crisis Communication Template:**
1. **What happened** (brief summary)
2. **Impact** (who/what is affected)
3. **Current status** (what's being done now)
4. **Action needed** (what should readers do)
5. **Next update** (when will you communicate again)

**Decision-Making Under Uncertainty:**
In crises, waiting for perfect information often creates more risk than making an informed decision with imperfect data. Develop the ability to:
- Assess confidence levels in available information
- Understand trade-offs and consequences of delay
- Make reversible decisions quickly, irreversible ones carefully
- Communicate uncertainty honestly while projecting confidence in the process

#### 12. Convert Crises into Organizational Learning

**Core Principle:**
> **Never waste a good crisis.** Every incident is an opportunity for organizational learning and systemic improvement. The post-mortem is more important than the incident response.

**Practical Application:**
- Always write post-mortems, even for "small" incidents
- Focus on learning, not blame ("blameless post-mortems")
- Extract actionable items, not just "we should be more careful"
- Track post-mortem action items to completion
- Share learnings broadly across the organization
- Look for patterns across multiple incidents
- **Embed mechanisms for continuous improvement**: Regular evaluation, learning from exercises, iterating on capabilities

**Red Flag:**
If you're experiencing the same type of incident repeatedly without systemic changes, you're not learning effectively.

**Continuous Improvement Framework:**
1. **Incident Response**: Handle the immediate crisis
2. **Post-Mortem**: Document what happened and why (within days)
3. **Root Cause Analysis**: Identify systemic issues, not just proximate causes
4. **Action Items**: Define specific, assigned, time-bound improvements
5. **Follow-Through**: Track action items to completion
6. **Pattern Recognition**: Analyze multiple incidents for themes
7. **Systemic Solutions**: Design solutions that prevent entire classes of problems

**Learning Culture:**
Facilitate post-mortems, retrospectives, and game days to create organizational rituals around learning. Promote experimentation and knowledge sharing as core values.

### Communication & Influence

#### 13. Adapt Communication for Different Audiences

**Core Principle:**
> **Your message doesn't matter if your audience can't understand it.** Master the art of translating between technical, business, and public communication styles.

**Practical Application:**
- **For executives**: Focus on business impact, risks, and strategic alignment
- **For engineers**: Include technical details, architecture, and implementation
- **For cross-functional partners**: Emphasize shared goals and collaboration points
- **For the public**: Focus on principles, outcomes, and broader implications
- **For internal comms**: Balance transparency with appropriate detail level
- **Tailor your message**: Adapt communication style and detail based on audience needs

**Communication Checklist:**
- Who is my audience?
- What do they need to know vs. want to know?
- What action do I want them to take?
- What level of technical detail is appropriate?
- What's the right tone (urgent, informative, celebratory)?

**Transparent Communication Principle:**
Ensure plans, priorities, risks, and progress are communicated clearly and proactively to relevant stakeholders. Be transparent about challenges and setbacks, along with plans to address them.

#### 14. Proactive Communication Builds Trust

**Core Principle:**
> **Proactive communication builds trust; reactive communication damages it.** Get ahead of security changes and incidents whenever possible.

**Practical Application:**
- Announce security changes well in advance (especially breaking changes)
- Explain the "why" behind security decisions, not just the "what"
- Share threat intelligence proactively (phishing warnings, etc.)
- Communicate early and often on strategic initiatives
- Be transparent about challenges and trade-offs
- **Develop a communication strategy**: Plan *how* and *when* to update different stakeholder groups

**Example:**
Giving 10 months advance notice before a major security requirement (like 2FA), with clear explanation of rationale and regular progress updates, can result in 95%+ voluntary adoption and maintained community confidence.

### Coalition Building & Cross-functional Work

#### 15. Build Coalitions Across Organizational Boundaries

**Core Principle:**
> **Transformational change requires coalition building, not just technical excellence.** No single team owns the customer experience; complex initiatives need cross-functional alignment. Large security initiatives fail without buy-in from non-security teams—you can't mandate security culture; you have to build it through partnerships.

**Practical Application:**
- Identify all stakeholders early (not just obvious technical partners; include technical and non-technical)
- Build relationships before you need them for a project
- Understand each team's goals, constraints, and success metrics
- Find shared wins, not just security wins
- Create communication channels and regular syncs
- Share credit broadly when successful
- Provide tools and support, not just requirements
- Measure impact on all stakeholders, not just security metrics
- **Master cross-functional collaboration**: Recognize that complex problems require partnership across teams, disciplines, and organizational boundaries

**Coalition Building Checklist:**
- Who needs to execute work for this initiative?
- Who needs to approve or provide resources?
- Who will be impacted by the change?
- Who has relevant expertise or context?
- Who might block or resist if not included?

**Communication Across Silos:**
Learn to translate technical concepts into language that resonates with different functions (Product, Design, Marketing, Sales, Legal). Understand their priorities and constraints. Facilitate joint planning sessions to ensure alignment.

**Security-Specific Coalition Building:**
Large-scale security transformations require particularly careful coalition building:
- **Engineering**: Provide secure-by-default tools and libraries
- **Product**: Show how security enables customer trust and sales
- **Support**: Ensure security changes don't create support burden (or reduce it)
- **Revenue**: Demonstrate security as competitive advantage
- **Communications**: Partner on messaging for security changes

### Process & Governance

#### 16. Fix Broken Processes, Don't Just Complain

**Core Principle:**
> **Complaining about broken processes is easy; fixing them is leadership.** When you identify systemic process failures, take ownership of the solution.

**Practical Application:**
1. **Diagnose**: Identify specific failure points (not just "it's broken")
2. **Design**: Create lightweight, sustainable alternative
3. **Deliver**: Implement with quick wins to build momentum
4. **Delegate**: Hand off to appropriate long-term owner
5. **Document**: Ensure sustainability beyond your involvement

**Red Flags in Processes:**
- High backlog of stale items
- Long cycle times frustrating requestors
- Unclear ownership or decision-making authority
- Bottlenecks on specific people
- No clear prioritization criteria

**Fix Pattern:**
- Clean up the backlog (often requires one-time effort)
- Establish clear SLAs and prioritization
- Distribute ownership (remove single points of failure)
- Measure and iterate

#### 17. Create Clear Planning Materials and Roadmaps

**Core Principle:**
> **Strategy without a plan is just wishful thinking.** Clear planning materials align teams, communicate priorities, and enable execution.

**Practical Application:**
- **Roadmaps should include**:
  - Clear objectives and key results (OKRs)
  - Timeline with milestones
  - Dependencies and blockers
  - Resource requirements
  - Success metrics
  - Risk assessment

- **Good planning materials are**:
  - Skimmable (execs can understand in 5 minutes)
  - Detailed enough for execution teams
  - Updated regularly (living documents)
  - Aligned with business priorities
  - Realistic about constraints

**Planning Principles:**
- Make trade-offs explicit
- Show work already in progress vs. new commitments
- Identify what you're *not* doing (equally important)
- Connect initiatives to business outcomes
- Update quarterly, but think in multi-year horizons

#### 18. Advocate for Standardization & Paved Paths

**Core Principle:**
> **Every team solving the same problem differently creates waste and risk.** Standardization enables efficiency, consistency, and quality—but only when implemented as "paved paths" that make the right way the easy way.

**Practical Application:**
- **Identify areas for standardization**: Look for inconsistencies or inefficiencies across teams (logging formats, deployment pipelines, security controls)
- **Define and document standards**: Work with stakeholders to create clear, well-documented standards and recommended practices
- **Build enabling tooling**: Advocate for tools and infrastructure that make standards easy to adopt
- Don't mandate standards without providing the tools to follow them
- Make the secure/correct path the default path
- Allow flexibility for legitimate exceptions

**Standardization vs. Innovation Balance:**
Standardize what's well-understood and repetitive (build, test, deploy, monitor). Allow flexibility where innovation and experimentation are needed (new product features, research areas).

**Paved Path Examples:**
- Automated security scanning in CI/CD (developers don't need to configure)
- Standard logging libraries with proper configuration (teams don't reinvent)
- Deployment templates with security controls built-in (secure by default)
- Pre-approved technology stacks and patterns (faster decisions)

### Career Development

#### 19. Build Broad Expertise Across Domains

**Core Principle:**
> **Senior IC and leadership roles require T-shaped skills: deep expertise in your domain plus broad understanding of adjacent areas.** Intentionally build breadth alongside depth.

**Practical Application:**
- Volunteer for projects outside your core expertise
- Shadow teams in adjacent functions (sales, support, product)
- Learn the business model and revenue drivers
- Understand compliance and regulatory landscape
- Develop communication skills (writing, presenting, facilitating)
- Build crisis management experience
- Learn process design and organizational dynamics

**Career Path Pattern:**
1. **Early Career**: Build deep technical expertise
2. **Mid Career**: Add breadth (team leadership, cross-functional work)
3. **Senior IC**: Leverage broad expertise for strategic impact
4. **Principal**: System-level thinking across technical, organizational, business domains

**For Aspiring Staff Engineers:**
Develop understanding of business strategy, product roadmap, and key results. Practice articulating how technical work contributes to strategic goals. Build relationships across functions, not just within engineering.

#### 20. Demonstrate Principal-Level Impact Before Promotion

**Core Principle:**
> **Promotions to senior levels are earned by performing at the next level, not by mastering the current level.** Show principal-level impact before the promotion, not after.

**Principal-Level Indicators:**
- **Scope**: Multi-year, company-wide strategic changes
- **Impact**: Measurable business outcomes (millions of users, elimination of vulnerability classes, revenue enablement)
- **Influence**: Industry recognition, external thought leadership
- **Leverage**: Success through empowerment and coalitions, not just personal execution
- **Complexity**: Navigate ambiguous, cross-functional, strategic challenges
- **System Thinking**: Architecture and process design, not just implementation

**Promotion Readiness Check:**
Ask your manager: "What would principal-level work look like in my role?"
Then go do that work before asking for the promotion.

#### 21. Transition Your Role as Your Career Evolves

**Core Principle:**
> **Your role should evolve as you grow, not stay static.** Actively seek transitions that leverage your accumulated expertise in new ways.

**Practical Application:**
- Every 2-3 years, reassess whether your role still challenges you
- Identify what you've mastered and what you want to learn
- Look for opportunities to apply expertise in new contexts
- Be willing to step back from execution to enable strategy
- Advocate for role changes that align with your growth

**Transition Patterns:**
- Technical → Technical + Management
- Management → Strategic IC
- Execution → Advisory
- Internal focus → External influence
- Reactive → Proactive → Strategic

**Red Flag:**
If you've been in the exact same role for 4+ years with no evolution, you may be stagnating.

### Security-Specific Lessons

#### 22. Security Incidents Are Opportunities for Trust Building

**Core Principle:**
> **How you handle security incidents matters more than preventing every incident.** Transparent, rapid response builds trust; opacity and delays destroy it.

**Practical Application:**
- Acknowledge incidents quickly (don't wait for perfect information)
- Communicate impact honestly (don't minimize or exaggerate)
- Provide clear guidance on actions users/employees should take
- Share learnings publicly when appropriate
- Fix the root cause, not just the symptom
- Use incidents to demonstrate security competence, not hide failures

**Trust-Building Incident Response:**
1. Fast acknowledgment
2. Clear impact assessment
3. Transparent communication
4. Decisive action
5. Thorough post-mortem
6. Systemic improvements
7. Public learning (when appropriate)

#### 23. Balance Security Rigor with Developer Experience

**Core Principle:**
> **Security that creates too much friction will be circumvented or ignored.** Design security controls that respect user workflows and provide clear value.

**Practical Application:**
- User research before implementing security controls
- Provide clear explanations of why security changes are needed
- Offer alternatives when possible (not just "no")
- Give advance notice for breaking changes
- Measure user impact (support tickets, adoption rates, workarounds)
- Iterate based on feedback
- Make the secure path the easy path
- **Build "paved paths"**: Make it easier to do the secure thing than the insecure thing

**UX Principles for Security:**
- **Secure by default**: Don't rely on users to configure security correctly
- **Clear value proposition**: Users should understand *why* a security control exists
- **Minimal friction**: Remove unnecessary steps or ceremony
- **Good error messages**: Tell users how to fix problems
- **Progressive disclosure**: Simple for simple cases, complexity available when needed

#### 24. Invest in Detection and Response, Not Just Prevention

**Core Principle:**
> **Prevention is ideal; detection and response are essential.** You cannot prevent every attack, so invest heavily in detection and response capabilities.

**Practical Application:**
- Build 24/7 incident response capabilities
- Practice incident response regularly (game days, tabletops)
- Measure MTTD (Mean Time To Detection) and MTTR (Mean Time To Response)
- Invest in monitoring, logging, and alerting
- Create playbooks for common incident types
- Test detection rules regularly (red team, purple team)
- Build automation for response tasks

**Security Investment Balance:**
- **Prevention**: Hardening, secure defaults, vulnerability management
- **Detection**: Monitoring, alerting, threat intelligence
- **Response**: Incident response, forensics, communication
- **Recovery**: Backup/restore, business continuity

**Reality Check:**
If you have no recent incident response practice, your detection and response capabilities are probably atrophied.

#### 25. Security Metrics Should Drive Action, Not Just Reporting

**Core Principle:**
> **Measure what matters and act on what you measure.** Security metrics should drive continuous improvement, not just satisfy compliance requirements.

**Practical Application:**
- Choose metrics that reflect actual security posture, not activity
- Set specific, measurable goals (zero secrets, <1hr MTTD, 95% adoption)
- Review metrics regularly with leadership
- Investigate adverse trends immediately
- Celebrate improvements publicly
- Adjust strategy based on metrics
- **Use data to inform planning and monitor progress** toward objectives

**Good Security Metrics:**
- **Leading indicators**: Vulnerability counts, secrets detected, phishing simulation results
- **Efficiency metrics**: MTTD, MTTR, time to patch critical vulnerabilities
- **Coverage metrics**: % of assets with security controls, % of code reviewed
- **Outcome metrics**: Incidents prevented, successful attacks, audit findings

**Bad Security Metrics:**
- Vanity metrics (number of security tools deployed)
- Activity metrics without outcomes (number of scans run)
- Metrics no one acts on

### Engineering Principles

#### 26. Technical Depth Enables Strategic Credibility

**Core Principle:**
> **Strategy without technical grounding is just buzzwords.** Stay technically current even as you move to strategic roles; credibility requires demonstrated expertise.

**Practical Application:**
- Continue hands-on technical work (even small projects)
- Stay current with technology trends in your domain
- Review technical designs and architecture docs
- Participate in technical discussions (not just strategy meetings)
- Test your strategic recommendations with real implementation work
- Be able to "go deep" when needed

**Credibility Test:**
Can you have a technical discussion with senior engineers and be respected as technically competent? If not, your strategic recommendations will be questioned.

#### 27. Leverage Automation Strategically

**Core Principle:**
> **Manual processes don't scale; automation does.** Invest in automation early to enable growth without linear headcount increases.

**Practical Application:**
- Identify high-volume, repetitive tasks
- Build automation incrementally (don't wait for perfect solutions)
- Create self-service tools for common requests
- Automate monitoring and alerting
- Use automation to enforce policies consistently
- Measure time saved and use it for higher-value work
- **Automate to reduce toil, improve efficiency, ensure consistency, and enforce standards**

**Automation Priority:**
1. **High-frequency tasks**: Things done multiple times per day
2. **Error-prone tasks**: Things humans do inconsistently
3. **High-stakes tasks**: Things where mistakes are costly
4. **Blocking tasks**: Things that are critical path for others

**Reality Check:**
If your team's capacity isn't growing faster than headcount, you're not automating enough.

#### 28. Document Everything (Especially Decisions)

**Core Principle:**
> **Undocumented decisions and processes are lost knowledge.** Document decisions, rationale, processes, and learnings—they become organizational assets.

**Practical Application:**
- Write post-mortems for all incidents (not just major ones)
- Document decision rationale in design docs
- Create runbooks and playbooks for common scenarios
- Maintain architecture decision records (ADRs)
- Write clear README files and wikis
- Document processes and handoffs

**What to Document:**
- **Decisions**: What was decided, why, what alternatives were considered
- **Processes**: Step-by-step guides for common tasks
- **Architecture**: System design, dependencies, trade-offs
- **Incidents**: What happened, root cause, fixes, learnings
- **Context**: Background information for future team members

**Documentation Quality:**
- Clear and concise (respect reader's time)
- Well-organized (easy to find relevant sections)
- Up-to-date (deprecated docs are worse than no docs)
- Actionable (reader can act on the information)

#### 29. Design for Failure and Proactive Mitigation

**Core Principle:**
> **Systems fail; humans make mistakes; attacks succeed.** Design systems, processes, and organizations that degrade gracefully and recover quickly. Shift from reactive to proactive approaches.

**Practical Application:**
- Assume breaches will occur (defense in depth)
- Build redundancy and backup processes
- Create clear escalation paths
- Test failure scenarios regularly (chaos engineering, incident drills)
- Design for graceful degradation
- Plan incident response before incidents occur
- Build recovery capabilities (backups, rollbacks, disaster recovery)
- **Proactively identify potential issues**: risks, capacity constraints, technical debt
- **Develop strategies to prevent or mitigate** before significant impact

**Resilience Principles:**
- **Redundancy**: No single points of failure
- **Monitoring**: Know when failures occur
- **Automated recovery**: Systems self-heal when possible
- **Clear escalation**: Humans intervene when needed
- **Practice**: Regular failure drills (game days)

**Proactive Planning:**
Conduct regular risk assessments in your domain. Anticipate future capacity needs, technical challenges, or security requirements based on business strategy and technical trends. Focus on prevention measures that stop problems before they occur.

#### 30. Incremental Progress Beats Perfect Solutions

**Core Principle:**
> **Perfect is the enemy of shipped.** Deliver incremental improvements consistently rather than waiting for perfect solutions.

**Practical Application:**
- Break large projects into shippable increments
- Deliver value early and often
- Iterate based on feedback
- Accept "good enough for now" when appropriate
- Prioritize 80% solutions that ship over 100% solutions that never launch
- Use phased rollouts to reduce risk

**Incremental Delivery Pattern:**
1. **MVP**: Minimum viable solution addressing core need
2. **Iteration**: Improve based on feedback
3. **Scale**: Expand to more users/use cases
4. **Polish**: Add nice-to-have features
5. **Maintain**: Keep working as context evolves

**Red Flag:**
If you've been working on something for >6 months without shipping anything, you're probably over-engineering.

### Legacy Building

#### 31. Build Organizational Capabilities, Not Personal Kingdoms

**Core Principle:**
> **Your legacy is what continues after you leave.** Build organizational capabilities, not personal indispensability.

**Practical Application:**
- Document your expertise (don't hoard knowledge)
- Develop successors for your role
- Create processes others can follow
- Build tools and frameworks for the organization
- Share credit and visibility
- Make yourself replaceable (it's a feature, not a bug)

**Legacy Questions:**
- If I left tomorrow, would my initiatives continue successfully?
- Have I developed others who can do what I do?
- Have I documented my knowledge and expertise?
- Have I created organizational assets (processes, tools, frameworks)?
- Am I building empire (dependency on me) or capability (organization can succeed without me)?

#### 32. Advocate for Investing in Core Capabilities

**Core Principle:**
> **Core capabilities are force multipliers; under-investment creates drag on everything else.** Advocate for necessary investment in foundational areas that enable future growth.

**Practical Application:**
- **Identify foundational needs**: Recognize where under-investment in core capabilities poses risks or hinders innovation
- **Build the case for investment**: Clearly articulate value and necessity, linking to risk reduction, future velocity, and business resilience
- **Champion infrastructure improvements**: Advocate for upgrades that support long-term platform health and scalability
- Connect infrastructure investments to business outcomes
- Show how foundational work enables future capabilities

**Core Capabilities Examples:**
- **Asset Inventory & Management**: Know what you have to protect
- **Logging & Monitoring**: Enables debugging, incident response, compliance
- **Business Continuity/Disaster Recovery**: Protects against catastrophic failures
- **Platform Services**: Foundational dialtone services that many teams depend on but are often taken for granted

**Investment Case Framework:**
1. **Current State**: What are the gaps or risks?
2. **Business Impact**: How does under-investment affect business outcomes?
3. **Proposed Investment**: What needs to be built/improved?
4. **Expected Benefits**: Risk reduction, velocity improvement, future enablement
5. **Cost of Inaction**: What happens if we don't invest?

#### 33. Industry Influence Extends Your Impact

**Core Principle:**
> **Your impact isn't limited to your employer.** Share learnings externally to influence industry practices and elevate your field.

**Practical Application:**
- Present at conferences (security, engineering, domain-specific)
- Write blog posts about lessons learned
- Engage with press on industry topics
- Speak at meetups and user groups
- Contribute to open source
- Mentor externally (not just within your company)
- Publish research and findings

**External Engagement Benefits:**
- **Industry influence**: Your work shapes best practices beyond your company
- **Talent attraction**: Public presence helps recruit great people
- **Personal brand**: Establishes you as domain expert
- **Learning**: Teaching forces deeper understanding
- **Network**: Build relationships across industry

#### 34. Model the Culture You Want to See

**Core Principle:**
> **Culture is built through consistent behavior, not policies.** Model the behaviors and values you want to see in your organization.

**Practical Application:**
- Be the incident responder you want on your team
- Write the documentation you wish existed
- Communicate the way you want others to communicate
- Show the work-life balance you want to normalize (I was admittedly not great at this one early in my career)
- Practice the learning mindset you want to encourage
- Demonstrate the collaboration you expect from others

**Culture Modeling:**
- **Psychological safety**: Admit mistakes publicly, ask for help
- **Learning**: Share what you learned from failures
- **Empowerment**: Give credit, delegate with trust
- **Clarity**: Communicate clearly and consistently
- **Accountability**: Own outcomes, good and bad

**Remember:**
Actions speak louder than policies. If you want a learning culture, model learning from your own mistakes.

---

### Core Planning & Strategy Principles

#### Summary: The 15 Principles from Formal Planning Documents

These principles consistently appear in effective strategic planning and complement the lessons above:

1. **Risk-First Perspective** (see Lesson 8): Prioritize based on identified risks and business impact
2. **Strategic Alignment** (see Lesson 9): Tie initiatives to organizational goals and business outcomes
3. **Clear Objectives & Measurable Outcomes** (see Lesson 10): Define SMART objectives with success metrics
4. **Bias for Action** (see Lesson 6, 11): Move quickly, make timely decisions, drive execution
5. **Cross-Functional Collaboration** (see Lesson 15): Partner across teams, disciplines, boundaries
6. **Long-Term Sustainability** (see Lesson 7): Build durable solutions that avoid "risk relapse"
7. **Continuous Improvement** (see Lesson 12): Embed learning, iteration, and evolution
8. **Accountability & Ownership** (see Lesson 2): Clear DRIs, governance frameworks, enforced responsibilities
9. **Data-Informed Planning & Monitoring** (see Lesson 25): Use metrics to understand state, track progress, measure effectiveness
10. **Proactive Planning & Mitigation** (see Lesson 29): Shift from reactive to proactive, identify issues early
11. **Standardization & Paved Paths** (see Lesson 18): Define standards, build enabling tools, make right way easy way
12. **Automation** (see Lesson 27): Reduce toil, improve efficiency, ensure consistency, enforce standards
13. **Customer & Ecosystem Focus** (see Lesson 9): Consider impact on internal/external customers and broader ecosystem
14. **Investing in Core Capabilities** (see Lesson 32): Advocate for foundational investments in critical areas
15. **Transparent Communication** (see Lessons 13-14): Ensure clear, proactive communication of plans, priorities, risks, progress

#### Integration Note

These 15 principles form the foundation of effective strategic leadership and are woven throughout the 34 detailed lessons above. They represent a consistent pattern of:
- **Risk-aware thinking** that connects to business outcomes
- **Strategic planning** with clear objectives and measurable results
- **Collaborative execution** that builds coalitions and empowers others
- **Sustainable solutions** that scale beyond individual heroics
- **Continuous improvement** through learning and iteration

Together, they demonstrate that **effective technical leadership requires both strategic thinking and tactical execution, deep technical expertise and broad business understanding, individual excellence and organizational capability building.**

---

### Summary: Core Leadership Principles

Synthesizing these lessons into core principles:

#### 1. **Empathetic Leadership**
- Model calm under pressure
- Empower others rather than centralizing control
- Mentor across levels and organizations
- Create psychological safety

#### 2. **Strategic Thinking**
- Think in 2-3 year horizons
- Identify systemic problems, not just symptoms
- Build coalitions for transformational change
- Balance strategic vision with tactical execution
- Embrace risk-first perspective with business alignment

#### 3. **Communication Excellence**
- Adapt to different audiences (technical, executive, public)
- Communicate proactively, especially on security topics
- Maintain clarity during crises
- Share learnings externally for industry impact
- Practice transparent communication of plans and progress

#### 4. **Process & Systems**
- Fix broken processes, don't just complain
- Build sustainable systems, not hero-dependent ones
- Document everything
- Design for failure and recovery
- Advocate for standardization and paved paths
- Leverage automation strategically

#### 5. **Career Growth**
- Build T-shaped expertise (deep + broad)
- Demonstrate next-level impact before promotion
- Transition roles as you grow

#### 6. **Legacy Building**
- Build organizational capabilities, not personal kingdoms
- Convert crises into learning
- Share knowledge widely
- Model the culture you want to see
- Invest in core capabilities
- Extend influence beyond your organization

#### 7. **Execution Excellence**
- Cultivate bias for action
- Set clear, measurable objectives
- Use data to inform decisions
- Practice proactive planning and mitigation
- Deliver incrementally with continuous improvement

---

### Final Reflection

Transformational impact in security and engineering leadership requires a combination of:

- **Technical credibility** (incident response, security architecture)
- **Strategic thinking** (multi-year initiatives with measurable impact)
- **Coalition building** (cross-functional partnerships)
- **Communication skills** (internal, external, crisis)
- **Empathetic leadership** (empowerment, mentoring, calm under pressure)
- **Process design** (sustainable systems and governance)
- **Risk-aware planning** (business-aligned, data-informed, proactive)

**The Core Lesson**: Impact at scale comes from **multiplying the efforts of others** (empowerment, processes, systems, culture) while maintaining **deep technical credibility and strategic vision**, all grounded in a **risk-first, business-aligned approach** to planning and execution.

Apply these lessons by:
1. **Building depth and breadth** in your expertise
2. **Focusing on systemic improvements**, not just point solutions
3. **Creating coalitions** for complex initiatives
4. **Communicating clearly** across audiences
5. **Modeling the culture** you want to see
6. **Building sustainable systems** that outlive your direct involvement
7. **Sharing learnings** externally for broader impact
8. **Embracing risk-aware, business-aligned strategic thinking**
9. **Cultivating bias for action** while maintaining long-term perspective
10. **Investing in core capabilities** that enable future success

---

**Document Purpose**: Practical guidance for security and engineering professionals, distilled from 9 years of security leadership experience at GitHub.

**Created**: November 3, 2025

**Author**: @swannysec (John Swanson, Hubber 2016-2025) with contributions in compilation from GitHub Copilot

