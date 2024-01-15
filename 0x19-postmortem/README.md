Postmortem: Calculator Compiler Outage
Issue Summary:
- Duration:
  - Start Time: January 13, 2024, 11:00 AM EAT
  - End Time: January 13, 2024, 1:00 PM EAT
- Impact:
  - The outage affected the parsing and evaluation of mathematical expressions, causing incorrect results and runtime errors for approximately 20% of users.
- Root Cause:
  - The root cause was identified as a bug in the parser that mishandled certain types of nested mathematical expressions.

 Timeline:
- 11:00 AM EAT:
  - Issue was detected as a result of automated testing, which revealed unexpected parsing errors and incorrect evaluation of expressions.
- 11:15 AM EAT:
  - Engineering team initiated investigation, suspecting a potential issue with the operator precedence handling in the parser.
- 11:45 AM EAT:
  - Misleading assumption led to an extensive review of the lexer component, consuming valuable time without identifying the root cause.
- 12:15 PM EAT:
  - Incident was escalated to the senior software engineer and the quality assurance team for additional support and expertise.
- 12:45 PM EAT:
  - Root cause was identified as a bug in the parser that mishandled certain types of nested mathematical expressions.
- 1:00 PM EAT:
  - The bug in the parser was fixed, resolving the parsing and evaluation issues.
Root Cause and Resolution:
- Cause:
  - The bug in the parser mishandled certain types of nested mathematical expressions, leading to incorrect results and runtime errors.
- Resolution:
  - The bug in the parser was fixed, ensuring correct parsing and evaluation of mathematical expressions.

Corrective and Preventative Measures:
- Improvements:
  - Enhanced unit testing to cover a wider range of nested expression scenarios.
  - Implementation of automated regression testing to detect similar parsing and evaluation issues in the future.
- Tasks:
  - Update the parser's handling of nested expressions to prevent similar mishandling in the future.
  - Implement automated regression testing for the parser to catch similar issues before they impact users.
  - Review and update incident response procedures to involve senior engineers and quality assurance earlier in the investigation process.

This outage served as a valuable learning experience, highlighting the importance of comprehensive testing, rapid cross-team communication, and automated regression testing to prevent similar incidents in the future.

By BIRIMUMASO ALFRED

