# User Workflow Journey: Parent Fund Management for Youth Account

## Experience Mindset

**Primary User:** Parent/Guardian

**Experience:** Managing a youth account (fund allocation, spending limits, activity monitoring)

**Scenarios Identified:**
1. Access youth account dashboard
2. Allocate funds to youth account
3. Set spending limit
4. View youth spending activity
5. Handle insufficient balance during fund allocation

---

## Scenario 1: Access Youth Account Dashboard

### Scenario 1A: Direct Navigation
- **Context:** Parent logs in and selects "Youth Account" from main dashboard
- **Action:** System loads youth account dashboard
- **Actor:** Parent
- **Goal:** Quickly access overview of youth account

### Scenario 1B: Notification-Driven Access
- **Context:** Parent receives notification about youth account activity and clicks link
- **Action:** System deep-links to youth account dashboard
- **Actor:** Parent
- **Goal:** Respond to specific activity or alert efficiently

#### User Goal
- Instantly view youth account status and recent activity

#### Business Goal
- Increase engagement and transparency for parental controls

#### Screens
1.0 Youth Account Dashboard

- **Page Goal:** Provide a comprehensive overview and quick access to management actions
- **Screen Description:**
  - Displays youth account balance, recent transactions, spending limit, and quick actions (Add Funds, Set Limit)
  - Notification banners for important updates
- **Design Problems:**
  - HMW ensure parents can find key actions without confusion?
  - HMW surface critical alerts without overwhelming the user?
- **Design Opportunities:**
  - What if dashboard widgets are customizable?
  - What if a summary of youth spending trends is shown?

**Screen Sequence:** 1.0 Youth Account Dashboard

---

## Scenario 2: Allocate Funds to Youth Account

### Scenario 2A: Standard Transfer
- **Context:** Parent on dashboard selects "Add Funds"
- **Action:** Initiates transfer from parent account to youth account
- **Actor:** Parent
- **Goal:** Move funds efficiently

### Scenario 2B: Quick Transfer from Notification
- **Context:** Parent receives low balance alert, clicks "Add Funds" in alert
- **Action:** Pre-fills transfer form with suggested amount
- **Actor:** Parent
- **Goal:** Resolve low balance with minimal steps

#### User Goal
- Seamlessly transfer funds to youth account

#### Business Goal
- Encourage regular funding and reinforce parental oversight

#### Screens
2.0 Fund Transfer Initiation
- **Page Goal:** Start the fund transfer process
- **Screen Description:**
  - Source account selector, amount input, youth account details
- **Design Problems:**
  - HMW minimize errors in amount entry?
  - HMW clarify which account is being debited?
- **Design Opportunities:**
  - What if smart suggestions for transfer amounts are provided?

2.1 Fund Transfer Confirmation
- **Page Goal:** Confirm transfer details before execution
- **Screen Description:**
  - Shows transfer summary, editable fields, confirm/cancel buttons
- **Design Problems:**
  - HMW prevent accidental transfers?
- **Design Opportunities:**
  - What if confirmation includes projected youth balance?

2.2 Fund Transfer Success
- **Page Goal:** Acknowledge successful transfer
- **Screen Description:**
  - Success message, updated balance, quick links to dashboard or set spending limit
- **Design Problems:**
  - HMW reinforce positive action?
- **Design Opportunities:**
  - What if a tip about teaching financial responsibility is shown?

Er.1 Insufficient Balance Error
- **Page Goal:** Communicate error and guide resolution
- **Screen Description:**
  - Error message, options to change amount or select different account
- **Design Problems:**
  - HMW reduce frustration when errors occur?
- **Design Opportunities:**
  - What if alternate funding options are suggested?

**Screen Sequence:** 1.0 Dashboard -> 2.0 Transfer Initiation -> 2.1 Confirmation -> 2.2 Success / Er.1 Error

---

## Scenario 3: Set Spending Limit

### Scenario 3A: Manual Limit Entry
- **Context:** Parent navigates to "Set Spending Limit" from dashboard
- **Action:** Enters weekly limit
- **Actor:** Parent
- **Goal:** Control youth spending

### Scenario 3B: Guided Limit Setup
- **Context:** Parent uses guided wizard with educational tips
- **Action:** System suggests limits based on age or spending history
- **Actor:** Parent
- **Goal:** Make informed decision

#### User Goal
- Easily configure and understand spending limits

#### Business Goal
- Promote responsible youth spending and parental peace of mind

#### Screens
3.0 Spending Limit Configuration
- **Page Goal:** Allow parent to set or edit weekly spending limit
- **Screen Description:**
  - Input field, current limit display, contextual guidance, save/cancel
- **Design Problems:**
  - HMW prevent invalid or extreme values?
  - HMW explain the impact of limits?
- **Design Opportunities:**
  - What if visualizations show how limits affect spending?

3.1 Limit Confirmation
- **Page Goal:** Confirm new limit
- **Screen Description:**
  - Summary of new/old limits, confirmation action
- **Design Problems:**
  - HMW ensure parent confidence in changes?
- **Design Opportunities:**
  - What if parent can set alerts for limit breaches?

**Screen Sequence:** 1.0 Dashboard -> 3.0 Limit Config -> 3.1 Confirmation

---

## Scenario 4: View Youth Spending Activity

### Scenario 4A: Standard Activity View
- **Context:** Parent selects "Activity" from dashboard
- **Action:** Sees transaction list
- **Actor:** Parent
- **Goal:** Monitor youth spending

### Scenario 4B: Filtered/Custom View
- **Context:** Parent applies filters (date, merchant, amount)
- **Action:** Sees tailored transaction list
- **Actor:** Parent
- **Goal:** Identify patterns or issues

#### User Goal
- Quickly scan and understand youth spending

#### Business Goal
- Increase parental trust and encourage financial education

#### Screens
4.0 Activity List
- **Page Goal:** Display youth account transactions
- **Screen Description:**
  - List with date, merchant, amount, remaining balance; filter controls
- **Design Problems:**
  - HMW make patterns visible at a glance?
  - HMW support accessibility for all parents?
- **Design Opportunities:**
  - What if spending categories are color-coded?
  - What if insights or tips are surfaced based on activity?

**Screen Sequence:** 1.0 Dashboard -> 4.0 Activity List

---

## Scenario 5: Handle Insufficient Balance During Fund Allocation

### Scenario 5A: Inline Error Handling
- **Context:** Parent enters amount exceeding available balance
- **Action:** Error shown inline, disables transfer
- **Actor:** Parent
- **Goal:** Correct error without leaving flow

### Scenario 5B: Alternative Account Suggestion
- **Context:** Parent's primary account lacks funds
- **Action:** System suggests alternate funding sources or prompts to add funds
- **Actor:** Parent
- **Goal:** Resolve issue and complete transfer

#### User Goal
- Understand and resolve funding issues efficiently

#### Business Goal
- Reduce failed transactions and support positive experience

#### Screens
Er.1 Insufficient Balance Error (as above)
- **Page Goal:** Clearly communicate issue and next steps
- **Screen Description:**
  - Error message, actionable suggestions
- **Design Problems:**
  - HMW avoid user frustration?
- **Design Opportunities:**
  - What if system offers to schedule transfer when funds are available?

**Screen Sequence:** 2.0 Transfer Initiation -> Er.1 Error

---

# Workflow Screen Sequences (Summary)

**Scenario 1:** 1.0 Dashboard

**Scenario 2:** 1.0 Dashboard -> 2.0 Transfer Initiation -> 2.1 Confirmation -> 2.2 Success / Er.1 Error

**Scenario 3:** 1.0 Dashboard -> 3.0 Limit Config -> 3.1 Confirmation

**Scenario 4:** 1.0 Dashboard -> 4.0 Activity List

**Scenario 5:** 2.0 Transfer Initiation -> Er.1 Error

---

# Accessibility & Scalability Considerations
- All screens designed for keyboard navigation and screen reader compatibility
- Color contrast and font sizes meet WCAG 2.1 AA
- Responsive layouts for desktop and tablet
- Modular design for future features (e.g., multiple youth accounts)

# Edge Cases & Additional Use Cases
- Parent with multiple youth accounts: dashboard supports account switching
- Youth account closed: dashboard displays closure status and historical data
- Parent attempts action while offline: system provides offline messaging and retry options

---

# End of Workflow Documentation
