# GitHub Workflows

This directory contains GitHub Actions workflows for automated CI/CD.

## Workflows

### 1. Deploy to GitHub Pages (`deploy.yml`)

**Trigger:** Push to `main` branch or manual workflow dispatch

**Purpose:** Builds and deploys the website to GitHub Pages for production.

**Steps:**
- Checkout repository
- Setup Node.js v22
- Install dependencies with `npm ci`
- Build with Astro (`npm run build`)
- Upload and deploy to GitHub Pages

---

### 2. PR Preview Build (`pr-preview.yml`)

**Trigger:** Pull requests targeting the `main` branch (opened, synchronized, or reopened)

**Purpose:** Automatically builds and validates PRs, providing preview artifacts and error reporting.

#### Features

##### ✅ Successful Builds
- Builds the Astro site and captures any issues
- Uploads build artifacts for review (retained for 7 days)
- Posts a success comment on the PR with artifact details and workflow links

##### ❌ Failed Builds
- Captures detailed error logs from installation or build steps
- Automatically posts the error log as a PR comment for easy debugging
- Logs are expandable and truncated if too long (max 60,000 characters)
- Updates existing bot comments instead of creating duplicate comments

#### How It Works

1. **Installation**: Runs `npm ci` and captures output to `install.log`
2. **Build**: Runs `npm run build` and captures output to `build.log`
3. **Artifact Upload**: On success, uploads the `dist` folder as a PR-specific artifact
4. **Error Reporting**: On failure, extracts error logs and posts them as a PR comment
5. **Status**: The workflow passes only if both installation and build succeed

#### Permissions

The workflow requires:
- `contents: read` - To checkout the repository
- `pull-requests: write` - To post comments on PRs
- `id-token: write` - For potential authentication needs

#### Example Comment (Success)

```
✅ Build Successful!

Your PR has been successfully built and is ready for preview.

📦 Artifact: pr-preview-123
🔗 Workflow Run: View Details

The build artifact is available for 7 days and can be downloaded from the workflow run.
```

#### Example Comment (Failure)

```
❌ Build Failed - Build Error

The build step failed for this PR. Please review the error log below:

📋 Click to view error log
[Expandable section with full error log]

🔗 Workflow Run: View Full Details

Please fix the errors and push your changes to trigger a new build.
```

#### Testing the Workflow

To test this workflow:
1. Create a new pull request targeting the `main` branch
2. The workflow will automatically trigger
3. Check the "Actions" tab to see the workflow run
4. Check the PR comments for build status and error logs (if any)

#### Troubleshooting

If builds are failing:
1. Check the PR comment for the specific error log
2. Click the workflow run link for full details
3. Fix the errors locally and push new commits
4. The workflow will automatically re-run on new commits

#### Customization

To modify the workflow:
- **Change Node version**: Edit the `node-version` in the Setup Node step
- **Adjust artifact retention**: Change `retention-days` in the Upload artifact step
- **Modify error log size**: Adjust `maxLogLength` in the error reporting script
- **Change trigger conditions**: Edit the `on:` section at the top of the workflow
