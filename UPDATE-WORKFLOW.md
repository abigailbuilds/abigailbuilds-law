# Law Site Update Workflow

This repository is set up as a fork of the main Abigail Builds website. Here's how to pull in design updates while preserving law-specific content:

## Setup Complete ✅
- Main site: `../Website` (upstream)
- Law site: `./` (current directory)
- Branch: `law-main` (for law-specific content)

## To Pull Design/Style Updates from Main Site:

### 1. Create a temporary branch for updates
```powershell
git checkout -b temp-upstream-update
```

### 2. Pull latest changes from main site
```powershell
git pull upstream main
```

### 3. Merge back to law-main, keeping law content
```powershell
git checkout law-main
git merge temp-upstream-update --no-commit
# Review changes, resolve conflicts (keep law content, accept design updates)
git add .
git commit -m "Update design from main site - [date]"
```

### 4. Clean up
```powershell
git branch -d temp-upstream-update
```

## Files to Watch During Merges:
- `index.html` - Keep law-specific content, accept design changes
- `styles.css` - Usually safe to accept all changes
- `script.js` - Usually safe to accept all changes
- `images/` - May need to keep law-specific branding

## Law-Specific Customizations Made:
- Hero section: Legal technology focus
- Trust strip: Law firm clients
- Services: Legal automation, practice management, etc.
- Meta tags: Legal SEO optimization

## Next Steps:
1. Continue customizing content for legal market
2. Add legal-specific case studies/projects
3. Update testimonials for law firm clients
4. Consider legal industry imagery
