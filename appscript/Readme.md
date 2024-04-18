# Google Sheets and GitHub Synchronization

## Summary
This repository contains code to synchronize data between a Google Sheet and a GitHub repository. The code consists of two main functions: `syncWithGitHub()` and `syncToGitHub()`. 

- `syncWithGitHub()`: Fetches data from a specified GitHub repository folder and updates a Google Sheet accordingly.
- `syncToGitHub()`: Pushes data from the Google Sheet to a specified GitHub repository folder.

## Generating a GitHub Token
To generate a GitHub token:
1. Go to your GitHub account settings.
2. Navigate to "Developer settings" > "Personal access tokens".
3. Click on "Generate new token".
4. Provide a token description and select the necessary scopes.
5. Click on "Generate token" and copy the generated token.

## Folder Location for Data Transmission
- **For `syncWithGitHub()`:** Update the `githubRepoUrl` variable to point to the desired folder in your GitHub repository from which data should be fetched.
- **For `syncToGitHub()`:** Update the `githubRepoUrl` variable to specify the target folder in your GitHub repository to which data should be pushed.

## Instructions for Using the Code
1. Open the Google Sheet associated with the project.
2. Go to "Extensions" > "Apps Script".
3. Paste the provided code into the script editor.
4. Save the script and grant necessary permissions.
5. Use the "Custom Menu" in the Google Sheet to execute the desired functions:
   - "Sync with GitHub": Fetches data from GitHub and updates the Google Sheet.
   - "Sync to GitHub": Pushes data from the Google Sheet to GitHub.

## Things to Remember While Modifying the Code
1. Ensure that the GitHub token is kept secure and not shared publicly.
2. Update folder locations (`githubRepoUrl`) with caution to avoid unintended data manipulation.
3. Review and test any modifications made to the code thoroughly before deployment to avoid errors or data loss.
