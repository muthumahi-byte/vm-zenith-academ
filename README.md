# VM ZENITH ACADEMY website

## Included
- Student page: enter name and class (1–12) to view Saturday/Sunday status.
- Admin page: password-protected login; set Tuition / Holiday / Not announced for each class and publish.
- Shared storage using Netlify Blobs, so published changes are visible to all visitors.
- Logo placeholder can be replaced later.

## Important setup
This project needs Netlify Functions and Netlify Blobs. A plain static upload of only `index.html` will NOT enable shared weekly updates.

1. Upload/extract this project into a GitHub repository, or deploy the folder using a Netlify-supported project workflow.
2. In Netlify, connect the repository and deploy. The included `netlify.toml` sets the publish folder and function folder.
3. In Netlify site settings, add an environment variable:
   - Key: `ADMIN_PASSWORD`
   - Value: choose a strong, private password (do not share it with students).
   Make sure the variable is available to Functions, then trigger a new deploy.
4. Open the deployed site. Use **Admin login** to sign in, choose statuses for all classes, and press **Publish weekly update**.
5. Students can then open the public page, enter their name and class, and see the published status.

## Update each week
Only change the Saturday and Sunday selections in the Admin area, then press Publish. You do not need to edit the code each week.

## Before public launch
Test the admin login and student status from a second device/browser. Keep the admin password private. Add the academy logo later by replacing the logo placeholder in `index.html`.
