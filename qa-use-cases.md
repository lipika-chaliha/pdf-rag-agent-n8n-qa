# RAG Use Cases for Software Testing

## 1. Requirements → Test Scenarios

Input:
- Requirement document
- BRD
- User stories

Possible output:
- Functional test scenarios
- Positive scenarios
- Negative scenarios
- Boundary conditions
- Missing requirement questions

## 2. BRD → Test Cases

The RAG Agent can retrieve the relevant business requirement and help draft test cases.

Possible output fields:

- Test Case ID
- Requirement
- Preconditions
- Test Steps
- Test Data
- Expected Result
- Priority

## 3. API Documentation → API Test Ideas

Input:
- API specification
- Endpoint documentation

Possible output:
- Happy-path tests
- Validation tests
- Authentication/authorization checks
- Boundary tests
- Error-response scenarios
- Negative API tests

## 4. Defect History → Defect Analysis

Input:
- Historical defects
- Root-cause notes
- Resolution information

Possible output:
- Similar historical defects
- Potential root causes
- Regression areas
- Suggested regression tests

## 5. Release Notes → Regression Testing

Input:
- Release notes
- Change summary
- Feature documentation

Possible output:
- Impacted modules
- Regression candidates
- Smoke-test candidates
- Risk-based test suggestions

## Example question

> Based on the uploaded requirement document, identify the main business rules and generate positive and negative test scenarios.

## Recommended QA guardrail

The AI output should be treated as an assistant-generated draft, not as a replacement for QA review.

A human tester should validate the retrieved context, assumptions, test coverage, and expected results before using the output in a real project.
