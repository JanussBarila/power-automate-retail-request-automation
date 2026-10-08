# Case Study Notes

## Problem

A multi-location retail business can receive operational requests from stores that require manual forwarding, approval and follow-up.

## Prototype

This proof of concept uses a structured Excel request register and Power Automate to:

- route requests by category;
- apply a cost-based approval rule;
- handle Approve and Reject outcomes;
- update request status;
- notify the relevant department.

## Current boundary

The project intentionally assumes that structured requests already exist in Excel. Request capture is not implemented in this version.

## Future phase

A production version could replace Excel with SharePoint Lists or Dataverse and add:

- Power Apps request form;
- SLA monitoring and escalation;
- requester notifications;
- Power BI management dashboard;
- AI-assisted classification and knowledge support.
