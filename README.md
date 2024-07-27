# cost-optimization--with--aws
AWS Cloud Cost Optimization - Identifying Stale Resources

In this mini project , a lambda fuction that identifies EBS snapshots that are no longer associated with any active EC2 instance will be created using a python code , the aim is to deletes them in order to save on storage costs.

Description:
The Lambda function fetches all EBS snapshots owned by the same account ('self') and also retrieves a list of active EC2 instances (running and stopped). For each snapshot, it checks if the associated volume (if exists) is not associated with any active instance. If it finds a stale snapshot, it deletes it, effectively optimizing storage costs.
