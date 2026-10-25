# CloudKickstart — Reproducible Static Website Deployment

## 1. Project overview
CloudKickstart is a small, beginner-friendly educational website that introduces cloud computing and three AWS services: Amazon EC2, Amazon S3, and AWS Amplify. It includes a simplified deployment workflow and a short interactive quiz.

## 2. Technologies used
- **HTML** — page structure and content.
- **CSS** — layout, colours, responsive styling.
- **JavaScript** — quiz interactions and score feedback.
- **GitHub** — source-code repository and version history.
- **AWS Amplify Hosting (planned deployment platform)** — hosting for the static website.

This project is a static website. It does not require a database, backend, package installation, or a build step.

## 3. Requirements
- A modern web browser.
- A GitHub account.
- An AWS account if deploying through AWS Amplify.
- Internet access to connect GitHub and the hosting platform.

## 4. Run the website locally
1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Test the navigation links and quiz.
4. No local server or extra dependencies are required for this simple static page.

## 5. Put the project on GitHub
1. Sign in to GitHub and create a new repository named `CloudKickstart`.
2. For a public learning project, make the repository public only after checking that it contains no private information or credentials.
3. Upload `index.html` and `README.md` to the repository root. The repository root should show both files directly.
4. Commit the changes to the `main` branch.
5. Open `index.html` from the repository and confirm the file is present.

GitHub's official guide to creating a repository: https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories

## 6. Deploy with AWS Amplify Hosting
These instructions describe the Git-connected workflow for a plain static HTML site.

1. Sign in to the AWS Management Console.
2. Open AWS Amplify Hosting: https://console.aws.amazon.com/amplify/
3. Choose the option to create/host a web app and select GitHub as the source provider.
4. Authorise the GitHub connection when prompted.
5. Select the `CloudKickstart` repository and the `main` branch.
6. Review the build settings. Because this project is plain HTML/CSS/JavaScript and has no build step, use the static-site settings appropriate for a project with `index.html` at the repository root. Do not add a framework build command that the project does not need.
7. Review the configuration and choose **Save and deploy**.
8. Wait for the deployment to complete, then open the generated public URL.
9. Test the URL in a private/incognito window or on another device. Check that the page loads and the quiz works.
10. Copy the final public URL into this README under **Live website URL**.

AWS's official guide: https://docs.aws.amazon.com/amplify/latest/userguide/welcome.html

**Note:** Console labels can change. If the current console presents different options, follow the current AWS Amplify Hosting documentation. Hosting may incur charges depending on usage; review current AWS pricing and remove resources you no longer need.

## 7. Alternative hosting option
If AWS Amplify is unavailable, GitHub Pages is an alternative for a static site:

1. Open the GitHub repository.
2. Go to **Settings → Pages**.
3. Choose deployment from a branch.
4. Select the `main` branch and the root folder, then save.
5. Wait for publication and open the URL shown by GitHub Pages.
6. Test the site and add its URL below.

Official guide: https://docs.github.com/en/pages/quickstart

## 8. Live website URL
- **Status:** Not deployed yet.
- **URL:** Add the actual public URL here after a successful deployment.

Do not claim a live URL until the site has actually been deployed and tested.

## 9. Security and good practices
- Never commit passwords, AWS access keys, API keys, or other secrets to a repository.
- Enable multi-factor authentication (MFA) on accounts.
- Use least-privilege access: grant only the permissions required.
- Review hosting charges and remove unused resources.
- Keep the README accurate if deployment steps or platform interfaces change.

## 10. Troubleshooting
- **The page does not load:** Check that `index.html` is in the repository root and the deployment completed successfully.
- **The deployment fails:** Read the deployment log, check the selected branch and hosting settings, and consult the official AWS documentation.
- **The site looks outdated after an edit:** Confirm that the latest changes were committed to the branch connected to hosting and that a new deployment completed.
- **The quiz does not work:** Open the browser's developer console and check for JavaScript errors.

## 11. What I learned
Use this section after following the steps and write your own honest reflection. Possible topics include the difference between local files and hosted websites, the role of GitHub in storing source code, how a hosting platform publishes a site, and how deployment errors are investigated.
