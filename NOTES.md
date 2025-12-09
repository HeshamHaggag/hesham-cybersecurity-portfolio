# Insecure Direct Object Reference (IDOR) – Example Notes

Scenario:
- Parameter `user_id` or `invoice_id` can be modified to access other users' data.

Approach:
- Change numeric IDs step by step in authorized test accounts
- Check access control validation

Mitigation:
- Enforce proper authorization checks on the server side
- Use indirect references or access control checks per object
