# Saanvi – AI Voice Agent for Home Credit

## 1. Project Overview

This project demonstrates a no-code AI voice agent built using **Bolna AI** for preliminary Loan Against Property (LAP) eligibility screening for existing Home Credit customers.

The voice agent, named **Saanvi**, conducts conversations with customers, verifies their identity before discussing offer details, collects eligibility information, validates responses, handles objections, and determines whether a customer can proceed to a senior loan expert.

The project includes the system prompt, detailed call logs, test cases, audio recording links, and conversation transcripts.

## 2. Project Objectives

- Develop an AI voice agent using a no-code platform.
- Automate preliminary eligibility screening through voice conversations.
- Collect and validate seven required eligibility criteria.
- Handle disqualification scenarios and customer objections.
- Route existing loan-transfer enquiries to the appropriate specialist.
- Handle wrong-number responses, unclear answers, customer refusals, and callback requests.
- Test the voice agent across 12 scenarios.
- Maintain supporting call records, timestamps, test case details, transcripts, and audio recording links.

## 3. Technology Used

| Component | Purpose |
|---|---|
| Bolna AI | No-code voice agent platform |
| AI System Prompt | Defines the agent's identity, conversation flow, rules, and responses |
| CSV Call Logs | Stores call records and associated details |
| Microsoft Word | Documents the system prompt, test cases, links, and transcripts |
| GitHub | Hosts the project documentation and deliverables |

## 4. Agent Details

- **Agent Name:** Saanvi
- **Platform:** Bolna AI
- **Use Case:** Preliminary Loan Against Property eligibility screening
- **Organisation Referenced:** Home Credit
- **Maximum Preliminary Loan Amount:** ₹75 lakh
- **Eligible Tenure:** 3–15 years, inclusive
- **Interaction Type:** AI-powered voice conversation

## 5. Eligibility Criteria

The agent collects and validates the following seven eligibility items.

| No. | Criterion | Eligibility Rule |
|---|---|---|
| 1 | Property Type | Residential, commercial, and industrial properties are allowed. Agricultural property is disqualified. |
| 2 | Property Ownership | Sole and joint ownership are accepted. |
| 3 | Original Property Documents | Original property documents must be available. |
| 4 | Loan Amount | The requested amount must not exceed ₹75 lakh. If the customer requests more, the agent explains the limit and asks whether the customer agrees to proceed at ₹75 lakh. |
| 5 | Occupation and Income | Salaried and self-employed customers are accepted if income is received through a bank. Income received entirely in cash is disqualifying. |
| 6 | Estimated Property Value | The agent records the customer's estimated current property market value. No minimum property-value threshold is specified in the assignment rules. |
| 7 | Loan Tenure | The accepted tenure range is 3–15 years, inclusive. Invalid tenures must be corrected before qualification can proceed. |

A customer is referred for the next stage only after all seven required items have been captured and validated.

## 6. Conversation Flow

The agent follows a structured conversation process:

1. Introduces itself and verifies the intended customer's identity.
2. Explains the preliminary offer only after identity verification.
3. Checks whether the customer is interested in continuing.
4. Collects property type and ownership details.
5. Checks the availability of original property documents.
6. Collects the requested loan amount and confirms acceptance of the ₹75 lakh limit when necessary.
7. Collects occupation and verifies the income mode.
8. Records the estimated property market value.
9. Collects and validates the requested loan tenure.
10. Determines whether the customer meets the preliminary criteria.
11. Provides the appropriate closing response or specialist referral.

## 7. Disqualification and Special Handling

The agent follows specific rules for the following situations:

- **Agricultural property:** Ends the fresh-loan qualification flow.
- **Original documents unavailable:** Ends the fresh-loan qualification flow.
- **Cash-only income:** Ends the fresh-loan qualification flow.
- **Loan amount above ₹75 lakh:** Explains the maximum limit and proceeds at ₹75 lakh only after explicit customer acceptance.
- **Customer declines the maximum amount:** Politely closes the conversation.
- **Invalid tenure:** Requests a valid alternative; closes the qualification flow if the customer insists on an invalid tenure.
- **Existing loan or transfer enquiry:** Routes the customer to the relevant transfer specialist instead of continuing the fresh-loan assessment.
- **Customer is busy:** Asks for a preferred future callback date and time, without claiming that a callback is scheduled unless the system supports it.
- **Wrong person answers:** Ends the call without disclosing private customer or offer information.
- **Unclear response:** Asks for clarification before making an eligibility decision.
- **Customer refuses the offer:** Respects the decision and closes politely.

## 8. Repository Files

The project contains the following deliverables.

| File Name | Description |
|---|---|
| `SYSTEM PROMPTS.docx` | Complete system prompt, Sections 1–10, defining the agent's identity, conversation flow, eligibility logic, closing branches, FAQs, objection handling, and variables. |
| `Saanvi-AI AGENT CALL LOGS.csv` | Detailed call log records, including call identifiers, date/time information, test case details, and other fields available in the exported call data. |
| `TESTCASES AND LINKS.docx` | The 12 test scenarios and corresponding audio recording links. |
| `TRANSCRIPTS.docx` | Written transcripts of the voice agent's test conversations. |

The file extensions above should match the actual files uploaded to the repository.

## 9. Call Logs and Recordings

The call log CSV is the main reference for reviewing the recorded test sessions.

It contains the detailed records exported for the calls, including the identifiers, date/time, test case information, and other recorded fields available in the export.

The `TESTCASES AND LINKS.docx` document provides the test scenarios and their corresponding audio recording links. The `TRANSCRIPTS.docx` document contains the written conversation transcripts.

Together, these deliverables allow a reviewer to examine the call records, read the conversations, and listen to the associated audio.

## 10. Test Cases and Validation

The voice agent was tested against 12 scenarios to evaluate its conversation flow, eligibility decisions, and handling of different customer responses.

| Test Case | Scenario | Expected Behaviour |
|---|---|---|
| TC-01 | Successful qualification | Collects and validates all seven criteria and provides the appropriate preliminary qualification closing. |
| TC-02 | Existing loan or transfer enquiry | Routes the customer to the transfer specialist and stops the fresh-loan flow. |
| TC-03 | Agricultural property | Disqualifies the customer from the fresh-loan flow. |
| TC-04 | Original property documents unavailable | Disqualifies the customer from the fresh-loan flow. |
| TC-05 | Income received entirely in cash | Disqualifies the customer from the fresh-loan flow. |
| TC-06 | Loan amount exceeds ₹75 lakh; customer declines the limit | Closes the conversation politely. |
| TC-07 | Loan amount exceeds ₹75 lakh; customer accepts the limit | Continues screening using ₹75 lakh after explicit acceptance. |
| TC-08 | Invalid tenure; customer insists on the invalid tenure | Requests a valid alternative and closes the qualification flow if the customer continues to insist. |
| TC-09 | Customer is busy | Asks for the preferred callback date and time without falsely claiming a confirmed booking. |
| TC-10 | Wrong person answers | Ends the call without revealing private information. |
| TC-11 | Unclear loan amount | Clarifies the amount before applying the loan amount rule and completing the screening. |
| TC-12 | Customer refuses the offer | Respects the customer's decision and ends the call politely. |

The detailed test document and call logs should be consulted for the actual recorded outcomes, timestamps, IDs, and recording links for each session.

## 11. How to Review the Project

1. Open `SYSTEM PROMPTS.docx` to understand the agent's instructions and eligibility rules.
2. Review `TESTCASES AND LINKS.docx` to understand the test scenarios and access their recordings.
3. Open `Saanvi-AI AGENT CALL LOGS.csv` to examine the recorded call details, identifiers, date/time values, and other exported information.
4. Read `TRANSCRIPTS.docx` to review the customer-agent conversations.
5. Compare the transcripts and recorded audio with the expected behaviour for each test case.

## 12. Important Limitations

- The agent performs preliminary eligibility screening only; it does not approve loans.
- Final approval and applicable interest rates are determined through the appropriate subsequent process.
- The agent must not invent interest rates, fees, minimum property-value thresholds, or other unverified loan terms.
- Customer acceptance of the ₹75 lakh limit must be explicit.
- Callback requests must not be represented as confirmed bookings unless supported by the system.
- The presence of a variable name in the prompt does not, by itself, mean that Bolna AI automatically creates or stores that variable.
- Test results describe the observed behaviour of the tested conversations and do not guarantee identical behaviour in every future call.

## 13. Privacy and Data Handling

Call logs, transcripts, and recordings may contain personal or customer-related information.

Before making the repository public:

- Remove or redact customer names, phone numbers, account-related information, and other personal data where necessary.
- Verify that the recordings and transcript links are permitted to be shared publicly.
- Do not upload credentials, API keys, access tokens, or confidential customer data.
- Use appropriately restricted sharing where public distribution is not authorised.

## 14. Submission Deliverables

The project submission includes:

- Complete system prompt containing Sections 1–10.
- Detailed call log CSV with the available call records and metadata.
- Test case document containing the 12 scenarios and audio links.
- Transcript document containing the written conversations.
- Audio recordings accessible through the supplied recording links.
- This README file documenting the project.

## 15. Disclaimer

This project is a demonstration of a no-code AI voice agent for preliminary eligibility screening. It is not a loan approval, a binding loan offer, or financial advice. All final lending decisions remain subject to the lender's applicable evaluation process.
