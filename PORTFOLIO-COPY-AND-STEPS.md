# Invoice Approval Automation: portfolio copy and publishing steps

This file is for you and is not part of the repo. Don't upload it to GitHub.

## Before you publish

- [ ] The Excel log fills correctly, so you can take the `excel-log.png` screenshot the README expects. The copy below describes the log as working.
- [ ] `flow-overview.png` and `excel-log.png` are in `docs/images/`. Crop out the browser tabs and address bar, and blank anything personal (tab titles, your name, the long environment code).
- [ ] You've exported the flow as `flow/InvoiceApproval.zip` with placeholder emails (build guide, "Document and publish" tab, step 2). If you'd rather not publish it, delete the `flow/` folder and the "Option A" line in the README.
- [ ] `docs/build-guide.md` is the build guide downloaded as Markdown.
- [ ] README placeholders filled in: `[time]`, your lessons, your LinkedIn link.

## 1. GitHub repo settings

| Setting | Value |
| --- | --- |
| Repository name | `invoice-approval-power-automate` |
| Visibility | Public |
| About description | Invoice approval workflow built with Power Automate, Microsoft Forms and Excel: amount-based routing, one-click approvals and an audit log. |
| Topics | `power-automate`, `microsoft-365`, `power-platform`, `automation`, `low-code`, `workflow` |
| Commit message | Add invoice approval automation project |

Upload everything inside the `invoice-approval-power-automate` folder, keeping the subfolders, and leave "Add a README" unticked.

## 2. Website project card

**Title:** Invoice Approval Automation

**One-liner:** An automated invoice approval workflow built on Microsoft 365, with amount-based routing, one-click approvals and a full audit log.

**Bullets:**
- Routes each invoice to the right approver by amount: over £750 to the CFO, everything else to the Sales manager
- Approvers approve or reject in Outlook or Teams, with a comment
- Every decision is logged in Excel and the submitter is emailed the outcome

**Tags:** Power Automate · Microsoft Forms · Excel · Microsoft 365 · Automation

**Image:** `flow-overview.png`

**Button:** View on GitHub, linking to `https://github.com/YOUR-USERNAME/invoice-approval-power-automate`

## 3. Short case study (for a project page)

**Problem.** Many small businesses still approve invoices over email and paper. Invoices get lost, suppliers get paid late, and there's no record of who approved what.

**What I built.** A Power Automate workflow. A supplier invoice is submitted through a Microsoft Form. The flow converts the amount to a number, picks the approver by value, sends an approve or reject request in Outlook or Teams, logs the decision in Excel and emails the submitter the outcome.

**Result.** I tested it with two fictional invoices. A £250 invoice went to the Sales manager and a £1,250 invoice went to the CFO, who rejected it with a comment. Each submitter received an email with the outcome.

**Security by design.** The form is restricted to signed-in users, each approval route has a named approver, every decision is timestamped, and the public repo contains no real data.

**What I learned.** Understand the process before automating it, because automating a bad process just makes mistakes faster. Forms returns every answer as text, so values need converting before you compare them. Next I'd add invoice attachments and an escalation if nobody responds.

## 4. CV and LinkedIn

**CV line (Projects):**
Invoice approval automation (Power Automate, Microsoft Forms, Excel): amount-based routing, one-click approvals and an audit log. Prototype built with fictional data. github.com/YOUR-USERNAME/invoice-approval-power-automate

**LinkedIn (Projects section):**
Built an invoice approval workflow in Power Automate. Invoices submitted through a Microsoft Form are routed to the right approver by amount, approved or rejected in Outlook or Teams, logged in Excel for audit, and the submitter is notified of the outcome. Documented on GitHub with a build guide and security notes.

## 5. Adding it to your portfolio site

Pick the option that matches how your site is built.

**A. Website builder (Wix, Squarespace, WordPress and similar)**
1. Open your Projects page and add a new item or card.
2. Upload `flow-overview.png` as the image.
3. Paste the title, one-liner and bullets from section 2.
4. Add a button labelled View on GitHub and link it to your repo.
5. For a full project page, paste section 3 and add the form, approval email and result email screenshots.
6. Publish, then open the page in a private window to check.

**B. Hand-coded HTML.** Copy `flow-overview.png` into your images folder and paste this into your projects section, matching your own class names:

```html
<article class="project-card">
  <img src="images/invoice-approval-flow.png" alt="Invoice approval workflow built in Power Automate">
  <h3>Invoice Approval Automation</h3>
  <p>An automated invoice approval workflow built on Microsoft 365, with amount-based routing, one-click approvals and a full audit log.</p>
  <ul class="tags">
    <li>Power Automate</li>
    <li>Microsoft Forms</li>
    <li>Excel</li>
    <li>Microsoft 365</li>
  </ul>
  <a href="https://github.com/YOUR-USERNAME/invoice-approval-power-automate">View on GitHub</a>
</article>
```

**C. Your GitHub profile is the portfolio.** Open your profile, click **Customize your pins**, and tick this repo. If you have a profile README, add a line such as: `Invoice Approval Automation: Power Automate workflow with routing, approvals and an audit log.`

If you tell me what your site is built with, I'll tailor this to it.

## 6. Final check (private window)

- [ ] The README renders, including the flow diagram
- [ ] All screenshots load
- [ ] No name, email, student ID or long environment code is visible anywhere
- [ ] The links to the build guide and sample CSV work
- [ ] The website button opens the repo
