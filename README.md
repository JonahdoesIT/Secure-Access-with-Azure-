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
Please view full project here https://jonahdoesit.github.io/Secure-Access-with-Azure-/
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


---

## 📚 References
- [Azure AD Documentation](https://learn.microsoft.com/en-us/azure/active-directory/)
