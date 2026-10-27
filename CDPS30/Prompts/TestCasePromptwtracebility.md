Master Prompt for ADO Import Test Case Generation:
 
Act as a Senior QA Consultant for CDPS applications, Azure DevOps Test Plans, Functional Testing, E2E Testing, Boundary Testing, Negative Testing, Integration Testing, and Database Validation.
 
Analyze the complete user story, acceptance criteria, business rules, field rules, conditional logic, error scenarios, UI behavior, dependencies, and design references provided.
 
Generate comprehensive Azure DevOps import-ready test cases in Excel format.
 
Requirements:
 
1. Test Coverage
Create test cases covering:
 
- End-to-End Happy Path scenarios
- Positive scenarios
- Negative scenarios
- Boundary Value Analysis
- Equivalence Partitioning
- Conditional Logic validations
- UI validations
- Dynamic field visibility validations
- Mandatory field validations
- Save as Draft scenarios
- Resume Application scenarios
- Session Timeout scenarios
- Database save failure scenarios
- API/service failure scenarios
- Application navigation failures
- System unavailable scenarios
- Accessibility validations where applicable
- Data persistence validations
- Integration validations
- Security validations for unauthorized access if applicable
 
2. ADO Format
 
Generate test cases in the exact Azure DevOps import structure below:
 
Work Item Type
Title
Test Step
Step Action
Step Expected
Area Path
Iteration Path
Assigned To
State
Coverage
 
3. Test Design Rules
 3.1. Each Test Case must be a parent row:
   Work Item Type = Test Case

3.2. Parent row:
   - Contains Test Case title
   - Test Step, Step Action and Step Expected must be blank

3.3. Child step rows:
   - Work Item Type blank
   - Title blank
   - Test Step contains 1, 2, 3, 4...
   - Step Action contains action
   - Step Expected contains expected result -don’t create reference – indicate the exact expected result 

- Each test case must be complete and executable independently.
- Create detailed step-by-step actions.
- Include expected results for every step. -don’t create reference – indicate the exact expected result 
- Use end-to-end journey format.
- Do not combine multiple validations into one test case.
- Create separate test cases for each business rule.
- Create separate test cases for each error scenario.
- Create separate test cases for each boundary condition.
- Create separate test cases for save draft and resume validations.
- Include database validation scenarios where data persistence is involved.
- Include service outage and recovery scenarios.
- Include field-level and page-level validations.
 
4. Coverage Mapping
 
Map every test case to:
- User Story
- Acceptance Criteria
- Error IDs
- Business Rules
- Field Rules
- Conditional Logic
 
using the Coverage column.
 
5. Test Case Naming Convention
 
Use:
 
TC001 E2E Happy Path
TC002 E2E Save Draft
TC003 Negative Validation
TC004 Boundary Validation
TC005 Database Failure
 
etc.
 
6. Output Requirements
 
Generate an ADO Excel (.xlsx) file.
 
Formatting:
 
- One worksheet named "ADO Import"
- Freeze header row
- Bold headers
- Auto-fit columns
- Wrap text enabled
- One row per test step
- Parent test case row followed by all associated steps
- Suitable for bulk import into Azure DevOps
 
7. Area Path
 
Use exactly:
 
Business Experience\CDPS Release 3.0\Stream1-Forms_Permit\S1_SOLGEN
 
8. Iteration Path
 
Use exactly:
 
Business Experience\CDPS Release 3.0\Sprint 2
 
9. Assigned To
 
Use exactly:
 
Wildo.laferte@ontario.ca
 
10. Final Deliverable
 
Provide:
 
- Downloadable Excel file
- Total test case count
- Coverage summary
- Traceability matrix showing:
    Requirement → Test Cases
    Acceptance Criteria → Test Cases
    Error IDs → Test Cases
 
Generate as many test cases as required to achieve 100% functional, negative, boundary, integration, and error coverage.
Ensure no acceptance criterion, business rule, field rule, conditional rule, or error scenario remains untested.


=================================================
TEST CASE TITLE TRACEABILITY REQUIREMENT
=================================================
Every Test Case title MUST include the source requirement.
Examples:
[AC] TC001 Verify Uniform Information Displayed For Security Guard Licence
[BR-001] TC002 Verify Uniform Information Applicable Only To Security Guard And Dual Licence
[BR-002] TC003 Verify Uniform Information Hidden For Private Investigator
[Flow] TC004 Verify Save As Draft Functionality
[Security] TC005 Verify Unauthorized Access Prevention
[Accessibility] TC006 Verify Keyboard Navigation
[DB Mapping] TC007 Verify Equipment Selections Persist To Application
[System Failure] TC008 Verify API Timeout Handling
Sources that may be referenced:
[AC]
[BR-001]
[BR-002]
[BR-003]
[BR-004]
[Flow]
[Validation]
[Integration]
[Security]
[Accessibility]
[Concurrency]
[DB Mapping]
[Responsive]
[Retention]
[System Failure]

