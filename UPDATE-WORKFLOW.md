# Abigail Builds Law - Standalone Repository

This is a separate repository for the law-focused version of the Abigail Builds website.

## Repository Setup ✅
- **Main site**: `abigailbuilds/abigailbuilds-website` (completely separate)
- **Law site**: `abigailbuilds/abigailbuilds-law` (this repository)
- **Branch**: `law-main` (main branch for law-specific content)

## Repository Information:
- **GitHub**: https://github.com/abigailbuilds/abigailbuilds-law
- **Website URL**: https://law.abigailbuilds.com/
- **Purpose**: Legal technology consulting services targeting law firms

## Development Workflow:

### 1. Standard Git Workflow
```powershell
# Make changes to files
git add .
git commit -m "Description of changes"
git push origin law-main
```

### 2. If you want to pull design updates from main site:
```powershell
# Add main site as a temporary remote
git remote add main-site https://github.com/abigailbuilds/abigailbuilds-website.git
git fetch main-site

# Create temporary branch for merging updates
git checkout -b temp-main-updates
git merge main-site/main --no-commit

# Review changes, keep law content, accept design updates
git add .
git commit -m "Merge design updates from main site"

# Merge back to law-main
git checkout law-main
git merge temp-main-updates

# Clean up
git branch -d temp-main-updates
git remote remove main-site
```

## Files Customized for Legal Market:
- ✅ **index.html**: Hero, services, practice areas, case studies
- ✅ **styles.css**: Practice areas styling
- ✅ **Meta tags**: Legal SEO optimization
- ✅ **Content**: Professional tone for law firm audience

## Law-Specific Features:
- ✅ 8 practice area specialties for SEO
- ✅ Legal compliance and security focus
- ✅ Professional, conservative tone
- ✅ Attorney-client privilege emphasis
- ✅ Case studies with legal context

## Next Steps:
1. Create the GitHub repository at `abigailbuilds/abigailbuilds-law`
2. Push the initial code
3. Set up hosting for `law.abigailbuilds.com`
4. Continue customizing content for legal market
