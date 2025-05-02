# osTicket-Congfiguration
how to configure osTicket before using it

## 🛠️ osTicket Setup Instructions

### ✅ Step 1: Acknowledge “User” vs “Admin” Panel
- **Admin:** [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)  
- **User:** [http://localhost/osTicket](http://localhost/osTicket)

---

### ✅ Step 2: Create “Supreme Admin” Role
- Admin Panel → **Agents** → **Roles**
  - Add new role: `Supreme Admin`
  - Assign **all** permissions, tasks, and knowledge

---

### ✅ Step 3: Create “Sys Admins” Department
- Admin Panel → **Agents** → **Departments**
  - Add new department: `Sys Admins`
  - Click **Create**

---

### ✅ Step 4: Configure a “Team”
- Admin Panel → **Agents** → **Teams**
  - Add new team: `Online Banking`
  - Click **Create**

---

### ✅ Step 5: Allow Anyone to Create Tickets (Even End Users)
- Admin Panel → **Settings** → **Users**
  - 🔲 Uncheck: `Require registration for users to open tickets`
  - Click **Save Settings**

---

### ✅ Step 6: Configure “Agents” (Workers)
- Admin Panel → **Agents** → **Add New**
  - Create **2 accounts**: Jane and John

**Jane Doe:**

&nbsp;&nbsp;&nbsp;&nbsp;Username: Jane  
&nbsp;&nbsp;&nbsp;&nbsp;Last name: Doe  
&nbsp;&nbsp;&nbsp;&nbsp;Email: Jane@gmail.com  
&nbsp;&nbsp;&nbsp;&nbsp;Password: Password1  
&nbsp;&nbsp;&nbsp;&nbsp;Department: Sys Admins  
&nbsp;&nbsp;&nbsp;&nbsp;Access: Supreme Admin  
&nbsp;&nbsp;&nbsp;&nbsp;Team: Online Banking

**John Doe:** Same as Jane, with John’s info.

> **Image:** "Users osTicket" — shows both agents + default "test Toad"




**John Doe:** Same as Jane, with John’s info.

> **Image:** "Users osTicket" — shows both agents + default "test Toad"

---

### ✅ Step 7: Add a User (Configure User)
- Agent Panel → **Users** → **Add User**
  - Email: `Karen@gmail.com`
  - Full Name: `Karen`

> **Image:** "Karen User" — shows Karen's account created

---

### ✅ Step 8: Configure SLA
- Admin Panel → **Manage** → **SLA**
  - Create 3 SLAs:
    - `Sev-A`: Grace Period: 1 hour, Schedule: 24/7  
    - `Sev-B`: Grace Period: 4 hours, Schedule: 24/7  
    - `Sev-C`: Grace Period: 8 hours, Schedule: Business Hours  

> **Image:** SLA Panel showing 3 new SLAs

---

### ✅ Step 9: Configure Help Topics (for Ticket Creation)
- Admin → **Manage** → **Help Topics**
  - Create the following help topics:

| Help Topic                  | Type             |
|----------------------------|------------------|
| Business Critical Outage   | Report a Problem |
| Personal Computer Issues   | Report a Problem |
| Equipment Request          | General Inquiry  |
| Password Reset             | Report a Problem |
| Other                      | General Inquiry  |

> **Image:** Help Topics Panel with entries listed above

---

### 🎉 Step 10: Finished!
Move to the next lab to start using osTicket.
