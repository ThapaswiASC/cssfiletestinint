# UX Workflow Documentation: Parent Fund Management for Youth Account

## Experience Mindset

**Primary User:** Parent or Guardian

**Experience:** Managing and teaching financial responsibility to a child via a youth banking account. This includes allocating funds, setting spending limits, monitoring activity, and handling errors (e.g., insufficient funds).

---

## Scenarios & Workflow Variations

### Scenario 1: Access Youth Account Dashboard
**Context:** Parent is logged in and wants to view/manage their child's account.

#### Variation A: Direct Navigation
- Parent selects "Youth Accounts" from main dashboard.
- Youth account dashboard loads with balance, recent activity, and quick actions.

#### Variation B: Notification-Driven Access
- Parent receives a notification (e.g., spending alert).
- Clicks notification, which deep-links to the youth account dashboard.

**User Goal:** Quickly access a comprehensive overview of the youth account.
**Business Goal:** Encourage regular parental engagement and trust in youth account features.

**Screens:**
1.0 Main Dashboard
2.0 Youth Account Dashboard

---

### Scenario 2: Allocate Funds to Youth Account
**Context:** Parent wants to add money to the youth account.

#### Variation A: From Dashboard Quick Action
- Parent clicks "Add Funds" on youth account dashboard.
- Fund transfer modal opens.
- Parent selects source account, enters amount, confirms transfer.
- Success or error message displayed.

#### Variation B: From Account Management Section
- Parent navigates to "Manage Accounts" > "Youth Account" > "Transfer Funds".
- Follows similar steps as above.

**User Goal:** Seamlessly transfer funds with confidence and minimal friction.
**Business Goal:** Promote use of youth accounts and reinforce parental control.

**Screens:**
2.0 Youth Account Dashboard
3.0 Fund Transfer Modal/Screen
Pu.1 Transfer Success
Er.1 Insufficient Balance Error

---

### Scenario 3: Set Spending Limit
**Context:** Parent wants to control weekly spending for the youth account.

#### Variation A: Inline Limit Setting
- Parent sees current limit on dashboard.
- Clicks "Edit Limit" inline.
- Edits value, sees contextual guidance, saves.
- Confirmation shown.

#### Variation B: Dedicated Limit Management Screen
- Parent navigates to "Manage Limits".
- Sets or edits weekly limit, reviews guidance, saves.
- Confirmation shown.

**User Goal:** Easily understand and set spending boundaries for their child.
**Business Goal:** Reduce risk of overspending, increase parental trust.

**Screens:**
2.0 Youth Account Dashboard
4.0 Limit Configuration Modal/Screen
Pu.2 Limit Update Success
Er.2 Invalid Limit Value Error

---

### Scenario 4: View Youth Spending Activity
**Context:** Parent wants to review their child's spending.

#### Variation A: Dashboard Activity Preview
- Parent sees recent transactions on dashboard.
- Clicks "View All" to see full activity list with filters.

#### Variation B: Filtered Activity Search
- Parent navigates to "Activity" tab.
- Uses filters (date, amount, merchant) to analyze spending patterns.

**User Goal:** Quickly identify spending patterns and spot issues.
**Business Goal:** Increase transparency and support financial education.

**Screens:**
2.0 Youth Account Dashboard
5.0 Activity List/Screen
5.1 Activity Filters

---

### Scenario 5: Handle Insufficient Balance During Fund Allocation
**Context:** Parent tries to transfer more than available in their account.

#### Variation A: Inline Error on Amount Entry
- Parent enters amount exceeding balance.
- Inline error message appears before submission.

#### Variation B: Error on Submission
- Parent submits transfer.
- Error modal appears, explaining insufficient funds and suggesting next steps.

**User Goal:** Understand why transfer failed and how to resolve it.
**Business Goal:** Reduce failed transactions, improve user satisfaction.

**Screens:**
3.0 Fund Transfer Modal/Screen
Er.1 Insufficient Balance Error

---

## Minimum Viable Experience (MVE)

### User Scenario Example
Sarah, a parent, wants to allocate $50 to her son’s youth account, set a $20 weekly spending limit, and review his recent purchases. She logs in, navigates to the youth account dashboard, adds funds, sets the limit, and checks the activity—all within a few clicks.

---

## Detailed Screen List & Documentation

### 1.0 Main Dashboard
- **Goal:** Entry point for all account management.
- **Description:** Shows summary of all accounts, notifications, and quick links to youth account.
- **Design Problems:**
  - HMW make youth account access prominent without clutter?
  - HMW balance information density for parents with multiple accounts?
- **Design Opportunities:**
  - What if the dashboard highlights youth account activity when action is needed?
  - What if a virtual assistant suggests next steps?

### 2.0 Youth Account Dashboard
- **Goal:** Central hub for youth account management.
- **Description:** Displays balance, recent activity, spending limit, and quick actions (Add Funds, Edit Limit).
- **Design Problems:**
  - HMW make key actions discoverable and accessible?
  - HMW communicate financial data clearly for quick scanning?
- **Design Opportunities:**
  - What if the dashboard adapts based on recent activity?
  - What if parents can set goals or challenges for their child?

### 3.0 Fund Transfer Modal/Screen
- **Goal:** Enable secure, simple fund transfers.
- **Description:** Source account selector, amount input, validation, confirmation, and feedback.
- **Design Problems:**
  - HMW prevent accidental transfers?
  - HMW communicate errors (e.g., insufficient funds) clearly?
- **Design Opportunities:**
  - What if the system suggests typical transfer amounts?
  - What if parents can schedule recurring transfers?

### 4.0 Limit Configuration Modal/Screen
- **Goal:** Allow parents to set and manage spending limits.
- **Description:** Editable weekly limit, contextual guidance, validation, and confirmation.
- **Design Problems:**
  - HMW explain the impact of limits to parents?
  - HMW prevent invalid or unrealistic limits?
- **Design Opportunities:**
  - What if the system recommends limits based on age or spending history?
  - What if parents can set temporary or event-based limits?

### 5.0 Activity List/Screen
- **Goal:** Provide detailed transaction history.
- **Description:** List of transactions with date, merchant, amount, and remaining balance. Filters for time period, amount, and merchant.
- **Design Problems:**
  - HMW make large lists easy to scan?
  - HMW help parents spot unusual activity?
- **Design Opportunities:**
  - What if the system flags suspicious transactions?
  - What if parents can categorize or annotate transactions?

### 5.1 Activity Filters
- **Goal:** Enable focused review of spending.
- **Description:** Filter controls for date range, amount, merchant, and type.
- **Design Problems:**
  - HMW keep filters simple but powerful?
- **Design Opportunities:**
  - What if filters can be saved as custom views?

### Pu.1 Transfer Success
- **Goal:** Confirm successful fund transfer.
- **Description:** Modal or toast with confirmation and updated balance.

### Pu.2 Limit Update Success
- **Goal:** Confirm successful limit update.
- **Description:** Modal or toast with confirmation and new limit.

### Er.1 Insufficient Balance Error
- **Goal:** Clearly communicate transfer failure due to insufficient funds.
- **Description:** Inline or modal error with actionable advice (e.g., "Reduce amount or add funds to your account.")

### Er.2 Invalid Limit Value Error
- **Goal:** Prevent and explain invalid limit entries.
- **Description:** Inline error with guidance on acceptable values.

---

## Sequence of Screens (Sample Flows)

### Fund Allocation Flow
1.0 Main Dashboard → 2.0 Youth Account Dashboard → 3.0 Fund Transfer Modal/Screen → Pu.1 Transfer Success / Er.1 Insufficient Balance Error

### Set Spending Limit Flow
1.0 Main Dashboard → 2.0 Youth Account Dashboard → 4.0 Limit Configuration Modal/Screen → Pu.2 Limit Update Success / Er.2 Invalid Limit Value Error

### View Activity Flow
1.0 Main Dashboard → 2.0 Youth Account Dashboard → 5.0 Activity List/Screen → 5.1 Activity Filters

---

## Accessibility & Scalability Considerations
- All actions are accessible via keyboard and screen reader.
- Color contrast and font sizes meet WCAG 2.1 AA standards.
- Responsive layouts for desktop and tablet.
- Modular design allows for future features (e.g., savings goals, rewards).

---

## Summary Table: Screens & Goals
| Screen ID | Title                        | Goal                                      |
|-----------|------------------------------|-------------------------------------------|
| 1.0       | Main Dashboard               | Entry point, quick access to youth acct   |
| 2.0       | Youth Account Dashboard      | Manage youth account, see overview        |
| 3.0       | Fund Transfer                | Transfer funds securely                   |
| 4.0       | Limit Configuration          | Set/manage spending limits                |
| 5.0       | Activity List                | Review transactions                       |
| 5.1       | Activity Filters             | Filter/sort transaction history           |
| Pu.1      | Transfer Success             | Confirm transfer                          |
| Pu.2      | Limit Update Success         | Confirm limit update                      |
| Er.1      | Insufficient Balance Error   | Explain transfer failure                  |
| Er.2      | Invalid Limit Value Error    | Prevent invalid limit                     |

---

*This documentation provides a systematic, user-centered workflow design for the parent fund management experience in youth banking, balancing user needs, business objectives, accessibility, and scalability.*
