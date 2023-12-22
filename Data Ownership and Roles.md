## Data Governance
- the processes an organization uses to manage, process, and protect data


## Access Control methods
### RBAC
- Role-Based Access Control
- (could be confused with Rule-based access control)

### Rule-based access control
- Rules are applied to people based on department]
- "Janitorial staff are allowed access to the building between 6 and 11PM on weekdays"
### ABAC
- **Attribute-Based Access Control** (**ABAC**)
- access is restricted based on an attribute of the account
- "if the user has (Condition X), then allow/deny them access to (data set D)"
### Group-Based Access Control
- If user is member of a group, they have access rights of that group

### MAC
- Mandatory Access Control
- data access control system based on classification rating
- commonly used in government/military applications

### MAC Roles

- **Owner**: the person who writes data, and the only person that can determine the classification.
- **Steward**: the person responsible for the quality and labeling of the data.
- **Custodian**: the person who stores and manages classified data. The custodian ensures the data is encrypted and backed up.
- **Security Administrator**: the person who gives access to classified data once clearance has been approved.


## Data roles

### Data owner 
- responsible for the confidentiality, integrity, availability, and privacy of information assets
- usually senior executives or somebody with authority and responsibility
- responsible for labeling the asset and ensuring that it is protected with appropriate controls
- The data owner normally selects the data steward and data custodian, and has the authority to direct their actions, budgets, and resource allocations

### Data steward 
- responsible for data quality
- ensures data is labeled and identified with appropriate metadata
- ensures data is collected and stored in a format and with values that comply with applicable laws and regulations

### Data custodian 
- manages the system on which the data assets are stored. 
- has responsibility for enforcing access control, encryption, and backup/recovery measures

### Privacy officer 
- responsible for oversight of any PII/SPI/PHI assets managed by a company