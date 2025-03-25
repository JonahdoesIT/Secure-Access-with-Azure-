# Secure Access with Azure Active Directory

## 🛡️ Project Overview
This project focuses on securing identity and access using **Azure Active Directory (Azure AD)** — now known as **Microsoft Entra ID**.

Key implementations:
- ✅ Multi-Factor Authentication (MFA)
- ✅ Conditional Access
- ✅ Role-Based Access Control (RBAC)
- ✅ Self-Service Password Reset (SSPR)
- ✅ User and Group Management

These practices help reduce unauthorized access risk and align with enterprise security standards.

---

## 🧱 Project Steps

### 🔹 Step 1: Create a New Azure AD Tenant
1. Log into the Azure Portal.
2. Select **Create a Resource** → Search for **Azure Active Directory** (Microsoft Entra ID).
3. Follow prompts to create a new tenant.



### 🔹 Step 2: Create New Users
1. Navigate to **Manage > Users** → Click **New User**.
2. Fill in details:
   - **Username**: `john@jonahland@ymail.onmicrosoft.com`
   - **Name**: John
   - **Password**: Use a strong password or auto-generate.
3. Repeat for:
   - **Dave**
   - **Jeff**

---

### 🔹 Step 3: Create a Group and Add Users
1. Go to **Manage > Groups** → Click **+ New Group**.
2. Select **Security** (or **Microsoft 365** depending on use case).
3. Name the group: `Dev Support`.
4. Under **Members**, click **+ Add Members** and add:
   - John
   - Dave
   - Jeff

---

### 🔹 Step 4: Enable Self-Service Password Reset (SSPR)
1. Navigate to **Manage > Password Reset > Properties**.
2. Set **Self-service password reset** to **Selected**.
3. Assign it to the `Dev Support` group.

---

### 🔹 Step 5: Test Self-Service Password Reset
1. Sign in with **Dave’s account**.
2. Go to **Security Info**.
3. Change the password.
4. ✅ Success: Password reset works!

---

### 🔹 Step 6: Enable and Enforce MFA
1. Navigate to **Manage > Users**.
2. Click **Per-user MFA** in the top menu.
3. In the MFA portal:
   - Select John, Dave, and Jeff.
   - Click **Enable**, then **Enforce** MFA for all users.
4. Confirm that MFA is required on next sign-in.

---

## 🧪 Outcome
- Users are protected by enforced MFA.
- SSPR is active for select users.
- Access and identities are organized using **Azure AD best practices**.

---

## 🧰 Tools Used
- Microsoft Azure / Entra ID
- Azure Portal
- Identity & Access Management (IAM)

---

## 📌 Notes
- Always assign the **Global Administrator** role to manage Azure AD settings.
- Regularly audit group memberships and MFA compliance.

---

## 📷 Screenshots
![Screenshot 2025-03-13 151259](https://github.com/user-attachments/assets/b3a324c5-2a8d-4fa2-a484-9b4a17f1cb3b)
![Screenshot 2025-03-13 154530](https://github.com/user-attachments/assets/c33a8ec2-fbd2-41b8-8144-18d72c457938)
![Screenshot 2025-03-13 155918](https://github.com/user-attachments/assets/e94e5ba9-966d-49e0-849f-1cb953f97952)
![Screenshot 2025-03-13 160255](https://github.com/user-attachments/assets/461e2f73-6d60-41c4-800f-6885150eaea3)
![Screenshot 2025-03-13 161239](https://github.com/user-attachments/assets/2eb6b8ec-73bc-4f84-ba40-5198ff471ee2)
![Screenshot 2025-03-13 162920](https://github.com/user-attachments/assets/a8a33f0b-a672-47ad-98bb-7d43ccc26259)
![Screenshot 2025-03-13 163123](https://github.com/user-attachments/assets/5bfd14f8-c7e6-488a-9fff-69054da5e9b8)
![Screenshot 2025-03-13 163814](https://github.com/user-attachments/assets/3b0ccb56-59c9-41df-bda7-69faaf78ab0f)
![Screenshot 2025-03-13 164020](https://github.com/user-attachments/assets/7a141fa0-eb99-4281-b8e4-424e1df297f8)
![Screenshot 2025-03-13 164539](https://github.com/user-attachments/assets/62ba4e3e-1ee0-47d9-8bbe-963e70e2d4eb)
![Screenshot 2025-03-13 164731](https://github.com/user-attachments/assets/d84e08eb-0a70-4d4b-8f28-314fd499f718)
![Screenshot 2025-03-13 165255](https://github.com/user-attachments/assets/31fbeed2-20f4-4779-aaf6-6c720584c789)
![Screenshot 2025-03-13 165339](https://github.com/user-attachments/assets/bcc4bb02-e52f-44e7-9a59-601bc6d72303)
![Screenshot 2025-03-13 201821](https://github.com/user-attachments/assets/9003714e-9693-4acf-b841-91b68f598b2a)
![Screenshot 2025-03-13 202118](https://github.com/user-attachments/assets/f891957b-af26-4744-84ac-719a9d34f069)
![Screenshot 2025-03-13 203134](https://github.com/user-attachments/assets/f6370bfb-fe20-47de-98eb-fb3409b945a8)
![Screenshot 2025-03-13 203601](https://github.com/user-attachments/assets/23aec7a7-010c-4203-8906-22f57bcdd8ce)
![Screenshot 2025-03-13 204008](https://github.com/user-attachments/assets/db081952-99a5-4590-b50e-3283580086f8)
![Screenshot 2025-03-13 204311](https://github.com/user-attachments/assets/28993194-b8ec-4957-8ab6-47ef77f49120)
![Screenshot 2025-03-13 204933](https://github.com/user-attachments/assets/7e1db556-6547-42bb-b064-7812bd9d126b)
![Screenshot 2025-03-13 205259](https://github.com/user-attachments/assets/d3ce1d8a-9874-4244-bb1f-4336a24b5b87)


---

## 📚 References
- [Azure AD Documentation](https://learn.microsoft.com/en-us/azure/active-directory/)
