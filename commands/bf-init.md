# /bf-init

Initialize your Budget Friend personal finance directory.

## Goal
Set up a secure, local folder for your financial documents and data so the agent can reference them consistently without you having to paste the same info repeatedly.

## 1. Setup Process
If you haven't already, create a dedicated folder for your finances (e.g., `~/Documents/my-finances`).

**To start initialization, tell the agent:**
"Run /bf-init in [path to your folder]"

## 2. The Interview (Grill Session)
The agent will now interview you to fill in the gaps. Be honest—the agent doesn't judge, it just calculates.

**The agent will ask about:**
- **Your Goal**: (e.g., "Get out of debt," "Save for a house," "Stop guessing my quarterly taxes").
- **Income Structure**: Regular salary? Freelance? Gig work? Irregular cycles?
- **Current State**: Do you have a budget? An emergency fund? A debt list?
- **Tooling**: How do you track money now? (Spreadsheets, apps, "it's all in my head").

## 3. Document Checklist
The agent will help you organize the following in your folder. 

**IMPORTANT: REDACT ALL SENSITIVE INFORMATION.** 
- Black out Account Numbers, SSNs, Passwords, and Full Names.
- Review your documents locally before providing them to the agent to ensure no sensitive data is uploaded to the cloud.

**Recommended Files:**
- **Bank Statements**: Exported as `.csv` (Preferred) or PDF.
- **Transaction Exports**: `.csv` from your bank or accounting software.
- **Tax Documents (Optional)**: Prior year returns (1040, Schedule C) to help with quarterly estimates.
- **Debt Logs**: A simple text file or CSV listing creditors, balances, and APRs.

## 4. Final Output
Once the interview and file check are done, the agent will create a `bf-profile.md` in your directory. This serves as your "Financial Source of Truth" for all future `/bf-*` commands.
