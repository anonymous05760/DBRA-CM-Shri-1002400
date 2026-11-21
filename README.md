**DBRA CM SHRI School, Khichripur **— School Portal & Private Student ERP
A web portal for DBRA CM SHRI School, Khichripur (School ID: 1002400) featuring a public-safe homepage and a restricted, role-based Student Academic & Bio-Data Registry unlocked exclusively for authenticated Teachers / Employees and the Principal.

Key Features
Zero Public Student Bio-Data Exposure: No student names, roll numbers, marks, attendance, or DBT/bio-data records are rendered in the DOM for unauthenticated visitors or Student logins.

Strict Role-Based Access Control (RBAC):

Unauthenticated / Student View: Displays only the Restricted Staff Portal lock notice (#erp-locked-banner).

Teacher / Employee & Principal View: Unlocks the private Student ERP Workspace (#erp-staff-workspace) upon role authentication.

Input-First Student Data Workflow: Starts empty (0 records) and prioritizes the Add / Input Student Record form so staff can enter records first before viewing or managing the registry.

CBSE Grading & Registry Controls:

Supports 1002400- student ID formatting, class, stream, house, attendance percentage, and DBT status.

Automatically computes CBSE-style grades from percentage/marks.

Provides search, class/stream filtering, inline edit/delete actions, CSV export, and audit activity logging for authorised staff.

Project Structure
Depending on how you organise your files, the portal consists of:

index.html — Portal layout, role login controls, restricted staff lock banner, student input form, registry table, and audit log UI.

style.css — Styling, layout hierarchy, role state visibility, and responsive components.

script.js — Role authentication state, form validation, CBSE grade calculation, CRUD operations, search/filter logic, CSV export, and audit trail handling.

(Note: In the single-file canvas output, HTML, CSS, and JavaScript are bundled together inside index.html.)

How to Use
Open the Portal: Launch index.html in a modern web browser (or serve it via a local static server / GitHub Pages).

Sign In as Staff: Select the Teacher / Employee or Principal role (or use the quick demo login option) to unlock #erp-staff-workspace.

Add Student Records: Fill out the Add / Input Student Record form and submit to add entries to the private registry.

Manage & Export: Use the search bar or class/stream filters to locate records, edit or remove entries as needed, review audit logs, or export the current registry to CSV.

Security & Privacy Notes
Client-Side Prototype Scope: If state is kept in browser memory or client-side storage without a backend session server, treat this as a front-end prototype rather than a production database.

Real Student Data: Avoid storing sensitive personal data (such as government IDs, contact details, or financial/DBT records) in unencrypted browser storage on shared or public computers.
