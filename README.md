# Home Credit LAP AI Voice Agent

## 1. Project Overview

This project involves building and testing an AI voice agent for Home Credit's Loan Against Property (LAP) qualification process using Retell AI. The agent conducts preliminary customer conversations, collects eligibility details, identifies ineligible cases, and refers eligible customers to a senior loan expert.

## 2. Tools Used

- Retell AI — voice agent configuration and call testing
- Large Language Model — conversational understanding and response generation
- GitHub — project documentation and system prompt
- Google Drive — audio recordings and transcripts

## 3. Agent Configuration

The agent was configured with a system prompt defining its role, conversation flow, qualification rules, and response guidelines. It was designed to handle interruptions, clarify unclear answers, retain previously provided information, and avoid promising final loan approval.

**Upload Screenshot 1 here:** `docs/images/agent-configuration.png`

## 4. Eligibility Rules

The agent checks the following requirements:

- Property must be residential, commercial, or industrial. Agricultural property is ineligible.
- Sole and joint ownership are accepted.
- Original property documents must be available.
- Maximum loan amount is ₹75 lakh.
- Income must be received through a bank account; cash-only income is ineligible.
- Estimated property market value must be collected.
- Repayment tenure must be between 3 and 15 years.
- Existing-loan transfer or EMI-reduction requests must be referred to the appropriate specialist.
- Eligible customers are referred to a senior loan expert. The agent does not provide final approval or invent interest rates.

## 5. Testing and Improvements

I tested the agent using nine simulated customer scenarios, including agricultural property, loan requests above the limit, callback requests, excessive tenure, missing documents, cash income, and eligible customers.

The tests helped identify areas requiring improvement:

- Ask explicitly whether the customer accepts ₹75 lakh when they initially request a higher amount.
- Clarify missing documents and mixed bank/cash income before determining eligibility.
- Avoid repeating questions when the customer has already provided a clear answer.
- Maintain a clear distinction between preliminary qualification and final loan approval.

The reviewed transcripts showed that some scenarios require further refinement and retesting before they can be considered fully successful.

## 6. Call History

Retell AI Call History was used to review test sessions, call durations, session status, and available call details.

**Upload Screenshot 2 here:** `docs/images/call-history.png`

## 7. Usage and Cost Monitoring

The billing dashboard was used to review call-related charges and remaining credits.

**Upload Screenshot 3 here:** `docs/images/billing-history.png`

The usage dashboard provided an overview of total cost, call minutes, average cost per minute, and provider costs during the displayed period.

**Upload Screenshot 4 here:** `docs/images/usage-analytics.png`

## 8. Project Links

- **System Prompt:** [Insert GitHub file link]
- **Test Recordings and Transcripts:** [Insert Google Drive folder link]
- **Retell AI Demo:** [Insert public demo link, if available]

## 9. Conclusion

This project demonstrates the configuration and testing of a voice agent for preliminary LAP qualification. Reviewing the test conversations helped identify improvements in eligibility validation, clarification handling, and adherence to business rules. Further testing is needed to verify fixes before deployment in a real customer environment.
