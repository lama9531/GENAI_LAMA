# My Final Project

## Project Name
Smart Meeting Follow-up Assistant
Lama ALqarani 
## Idea Selected

1. Meeting Follow-up Assistant


## Problem Statement
Meeting notes are often unorganized, which can lead to missed decisions, unclear tasks, and forgotten deadlines. This assistant helps organize meeting notes into clear summaries, decisions, action items, and follow-up messages.

## Target Users
Employees, team leaders, project managers, and administrative assistants who need to organize meeting notes and follow up on tasks and decisions.

## R-C-T-F Prompt
Role: Act as a professional meeting follow-up assistant.

Context: You will receive a CSV file containing meeting notes, tasks, responsible persons, deadlines, and status information.

Task: Analyze the file and identify the meeting summary, key decisions, action items, responsible persons, deadlines, open questions, and a short professional follow-up message.

Do not invent any missing information. If a responsible person or deadline is not provided, write “Not specified.”

Format: Organize the output into the following sections:

* Meeting Summary
* Key Decisions
* Action Items
* Open Questions
* Follow-up Message

For Action Items, use a table with:
Task | Responsible Person | Deadline | Status

## Sample Input
*Input File:* meeting_notes.csv

*Sample Data:*

The CSV file contains meeting information such as meeting date, meeting topic, notes, responsible person, deadline, and task status.

2026-10-01, Product Launch, Update website content, Ahmed, 2026-10-09, In Progress

2026-10-01, Product Launch, Prepare new product images, Sarah, 2026-10-05, Not Started

2026-10-01, Product Launch, Prepare and publish social media campaign, Not assigned, 2026-10-07, Not Started

2026-10-01, Product Launch, Confirm customer support training before launch, Not assigned, Not specified, Pending Decision
2026-10-01, Product Launch, Launch the new product, Team, 2026-10-10, Planned
## Sample Output
### Meeting Summary
The team is preparing for the product launch scheduled for October 10, 2026. The main tasks include updating the website, preparing product images, publishing a social media campaign, and confirming customer support training.

### Key Decisions
- The product launch is scheduled for October 10, 2026.
- The website must be updated before the launch.
- The social media campaign should be published before the launch.

### Action Items

| Task | Responsible Person | Deadline | Status |
|---|---|---|---|
| Update website content | Ahmed | October 9, 2026 | In Progress |
| Prepare new product images | Sarah | October 5, 2026 | Not Started |
| Prepare and publish social media campaign | Not specified | October 7, 2026 | Not Started |
| Confirm customer support training | Not specified | Not specified | Pending Decision |

### Open Questions
- Who will be responsible for the social media campaign?
- When will customer support training be confirmed?

### Follow-up Message
Hello Team,

Thank you for the meeting. Please continue working on the assigned tasks for the upcoming product launch. Sarah will prepare the product images by October 5, and Ahmed will update the website by October 9. The social media campaign still needs a responsible person, and the customer support training plan is still pending confirmation.

Best regards.

## Safety Checklist
- Do not upload confidential or sensitive company information to public AI tools.
- Review all AI-generated results before sharing them with the team.
- Do not allow the AI to invent missing names, deadlines, or decisions.
- Remove unnecessary personal information from meeting data.
- Use only approved AI tools according to company security policies.

## Reflection
This project helped me understand how generative AI can be used to improve workplace productivity.

I learned that using a clear R-C-T-F prompt helps the AI produce more organized, accurate, and useful results.

The Meeting Follow-up Assistant was able to analyze meeting data from a CSV file and convert it into a summary, key decisions, action items, open questions, and a professional follow-up message.
I also learned the importance of protecting sensitive data and reviewing AI-generated outputs before using or sharing them.
In the future, this project could be improved by connecting it to meeting tools so that meeting notes can be processed automatically.

## SDAIA Academy
GitHub: https://github.com/SDAIAAcademy
