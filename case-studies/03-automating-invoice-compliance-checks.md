# Automating invoice compliance checks for a multi-country freelancer network

*Real case, from two years at Le Wagon. No internal names.*

**Context**: over 60 freelance instructors submitting monthly invoices, across four countries (France, Germany, Spain, Portugal) and three legal statuses, each with different mandatory mentions, VAT rules, and calculation requirements. Checking them by hand took the operations lead half a day every month, with frequent errors and back-and-forth.

**What I did**: mapped every compliance rule with the operations lead first, twelve checks in total across the three statuses and four countries, plus about thirty edge cases. Built a knowledge base with every instructor's profile (status, country, applicable VAT) and every validation rule. Then built an agent that reads the invoice, runs all twelve checks in parallel, and posts a structured report with any flagged issue directly in the team's Slack channel. Tested it on ten real invoices before rolling it out, with a twenty-minute walkthrough instead of a training session.

**Result**: processing time per monthly batch went from about four hours to ten minutes. Error rate dropped by roughly 80%. Zero escalations in the eight months after launch. It became the most-used agent at Le Wagon, and other teams asked to adopt the same approach.
