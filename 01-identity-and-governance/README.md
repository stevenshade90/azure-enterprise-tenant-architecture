# Phase 1: Identity, Access Control, and Governance

## Business Scenario
'Practice Company' is a tech startup that focuses on automated inventory tracking for local retailers. To support operations, the Azure tenant will have four separate departments utilizing different groups and Administrative Units: IT & Security, Finance, Human Resources, and Engineering. 

## Step-by-Step Implementation
### Step 1: Add Users
Each department in the 'Practice Company' has hired a department head and 2-5 new employees. All employees were created and added to the Entra ID directory. 

## Step 2: Groups and Administrative Units
To avoid managing individual accounts, all employees were organized into appropriate security groups (e.g., 'IT-Staff-Group', 'HR-Staff-Group'). To reduce creation time, users were auto-assigned into each group using dynamic memberships. 

Administrative boundaries were set by implementing Administrative Units (AU). Each security group that was created was then managed by a specific AU. For example, the 'IT-Department-AU' was created and houses the 'IT-Staff-Group'. The Director of IT was then assigned the *User Administrator* role scoped to the AU, allowing the Director to have administrator control over the IT team and preventing the Director from accessing the other departments.
 
