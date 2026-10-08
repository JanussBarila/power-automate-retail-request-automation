# Power Automate Expressions

## Current row values

Request ID:
items('Apply_to_each')?['Request ID']

Category:
items('Apply_to_each')?['Request Category']

Status:
items('Apply_to_each')?['Status']

Priority:
items('Apply_to_each')?['Priority']

Description:
items('Apply_to_each')?['Description']

Estimated cost as number:
float(items('Apply_to_each')?['Estimated Cost EUR'])

## Approval

Approval outcome:
body('Start_and_wait_for_an_approval')?['outcome']

Approval title:
concat(
  'Approval required - ',
  items('Apply_to_each')?['Request ID'],
  ' - EUR ',
  string(items('Apply_to_each')?['Estimated Cost EUR'])
)
