# Bearer Token Detection Pre-commit Hook

A simple Git pre-commit hook that prevents committing files containing Bearer tokens.

## Quick Setup

1. **Copy the pre-commit script to your hooks directory**:
   ```bash
   # Navigate to your repository
   cd your-repository
   
   # Create hooks directory if needed
   mkdir -p .git/hooks
   
   # Copy the script
   cp ./.git-hooks/pre-commit .git/hooks/
   ```

2. **That's it!** The hook will now run automatically when you commit.

## What it does

- Scans staged files before each commit
- Detects patterns like `Bearer xyz123...`
- Blocks commits if tokens are found
- Shows you where the tokens are located

## When tokens are found

You'll see output like:
```
Found Bearer token in config.js, please remove before committing
15:   Authorization: 'Bearer abc123xyz'
Commit rejected: Please remove the Bearer tokens from the files above and try again.
```

Fix the issues and try committing again.

## Bypass (use with caution)

If needed, you can bypass the hook with:
```bash
git commit --no-verify
```

## Troubleshooting

- **Hook not running?** Check that it's executable: `chmod +x .git/hooks/pre-commit`
- **Issues with the script?** Review the pre-commit file and adjust as needed