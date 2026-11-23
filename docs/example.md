# Example: password reset

**Buyer request:** "Customers sometimes forget passwords. Allow them to reset their password using email. Turn this into a Jira-ready user story and identify missing decisions."

**Illustrative output (not a live-agent transcript):**

## Summary
Enable customers to reset forgotten passwords through email. Status: **Draft — needs Product Owner confirmation**.

## Story
As a registered customer, I want to reset my forgotten password using email so that I can regain account access without contacting support.

## Candidate acceptance criteria

```gherkin
Scenario: Request a password reset
  Given I am on the sign-in page
  When I request a password reset using my registered email
  Then I see a confirmation message
  And the account recovery process is initiated

Scenario: Expired link
  Given a password reset link has expired
  When I attempt to use it
  Then my password is unchanged
  And I am offered a way to request a new link
```

## Decisions to confirm

- How long should reset links remain valid?
- What password policy already exists?
- Should active sessions be invalidated after a reset?
- Does the team already have an email delivery service?
- Are there specific security or accessibility obligations?

## INVEST notes

Value and testability are evident. Story size, dependency on email infrastructure and estimability require team review. The story is **not ready for implementation** until key decisions are resolved.
