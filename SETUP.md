# Install the profile README and statistics

This kit is intended for the public GitHub profile repository named `ALRayed446`.

## 1. Upload the files

1. Open `https://github.com/ALRayed446/ALRayed446` (create a **public** repository with this exact name if it does not exist).
2. Upload the included `README.md` to the repository root.
3. Upload the `assets/` folder, keeping `assets/rayed-galaxy-animated.gif` at that exact path.
4. Upload `.github/workflows/generate-snake.yml`, keeping the nested path exactly as shown.
5. Commit the changes to the repository's default branch.

The profile README appears on your GitHub profile when the repository name matches your username, the repository is public, and a root-level `README.md` exists.

## 2. Run the contribution-snake workflow

1. Open the profile repository on GitHub.
2. Select **Actions**.
3. Choose **Generate contribution snake**.
4. Click **Run workflow** and confirm.
5. Wait for the workflow to finish, then refresh the repository. It should create `output/github-snake.svg` and `output/github-snake-dark.svg`.
6. If the workflow cannot push, open **Settings → Actions → General → Workflow permissions** and enable **Read and write permissions**, then rerun it.

The workflow is also scheduled to refresh daily. The snake section may show a broken image until the first successful run creates the SVGs.

## 3. How the statistics update

- **GitHub statistics and languages:** rendered from GitHub Stats Extended's public card service.
- **Streak:** rendered from the public Streak Stats service; includes contribution totals and current/longest streak.
- **Activity graph:** shows recent activity (the service defaults to the last 31 days).
- **Contribution snake:** generated and committed to this repository by the included GitHub Actions workflow.
- **Profile views counter:** optional. The commented-out line in `README.md` counts image requests, not unique visitors, so it is intentionally not enabled by default.

## Important limitations

- Public cards generally reflect public GitHub activity. Private contribution data may not be included by the public widget services.
- Third-party card services can be rate-limited or temporarily unavailable. If one widget stops loading, your README and repositories still work; remove or replace only that card.
- A green contribution square, streak, commit count, or language chart is not proof of code quality. For client trust, working projects, tests, useful documentation, and honest project status matter more.
- No personal access token is required for this basic setup. Never paste a token, password, or API key into your README or a workflow file.

## References

- GitHub profile README documentation: https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme
- GitHub Stats Extended: https://github.com/stats-organization/github-stats-extended
- GitHub Readme Streak Stats: https://github.com/DenverCoder1/github-readme-streak-stats
- GitHub Readme Activity Graph: https://github.com/Ashutosh00710/github-readme-activity-graph
- Contribution snake GitHub Action: https://github.com/Platane/snk
