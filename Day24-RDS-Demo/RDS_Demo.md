# Temporary RDS Demo and Cleanup

## Overview
This project involved creating a temporary Amazon RDS MySQL instance (temp-demo-mysql) for demonstration purposes, connecting to it using a MySQL client / RDS Query Editor, and then deleting the instance and snapshots to prevent any further costs.

## Steps Followed

1. **RDS Instance Creation:**
   - Engine: MySQL (Free tier)
   - Instance Identifier: temp-demo-mysql
   - Instance Class: db.t2.micro
   - Deletion Protection: Disabled

2. **Testing:**
   - Connected via the RDS Query Editor and ran:
     ```sql
     SHOW DATABASES;
     ```
   - Verified that built-in databases were returned.

3. **Cleanup:**
   - Deleted the RDS instance without creating a final snapshot.
   - Verified and deleted any remaining snapshots via the RDS console.

## Observations
- The RDS instance worked as expected.
- Cleanup is essential to avoid inadvertent charges.
