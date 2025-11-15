# GitHub Pages Setup - Next Steps

## ✅ What's Been Done

1. **Jekyll Resume Template Installed** - Using the template from jglovier/resume-template
2. **Content Populated** - Your resume data from RESUME.pdf has been added:
   - Work Experience: Stride, Casebook PBC, Casecommons, and earlier roles
   - Skills: Java, TypeScript, React, Ruby, Node.js, and more
   - Projects: Peak Reservations, Peloton, Allied World, IBM, California & Indiana child welfare systems
   - Education: B.S. Computer Science from Curtin University
3. **Avatar Configured** - Nate.PNG has been set as your profile image
4. **Domain Setup** - CNAME file configured for drnatejones.com
5. **All Changes Committed** - Ready to push to GitHub

## 🚀 Next Steps to Deploy

### 1. Push to GitHub
```bash
git push origin master
```

### 2. Enable GitHub Pages
- Go to: https://github.com/cohesivejones/cohesivejones/settings/pages
- Under "Source", select branch: `master`
- Click "Save"

### 3. Configure Your Domain (drnatejones.com)

#### In GitHub:
- In the Pages settings, enter `drnatejones.com` in the Custom domain field
- Save the changes

#### In Your Domain Registrar (where you manage drnatejones.com):
Add these DNS records:

**A Records** (for apex domain):
```
Type: A
Name: @ (or leave blank)
Value: 185.199.108.153

Type: A
Name: @ (or leave blank)
Value: 185.199.109.153

Type: A
Name: @ (or leave blank)
Value: 185.199.110.153

Type: A
Name: @ (or leave blank)
Value: 185.199.111.153
```

**CNAME Record** (for www subdomain - optional):
```
Type: CNAME
Name: www
Value: cohesivejones.github.io
```

### 4. Wait for DNS Propagation
- Usually takes 15 minutes to 2 hours
- Can take up to 24-48 hours in rare cases
- Check status: https://www.whatsmydns.net/

### 5. Enable HTTPS
- Once domain verification succeeds in GitHub Pages settings
- Check "Enforce HTTPS"

## 🧪 Test Locally Before Pushing (Optional)

```bash
bundle install
bundle exec jekyll serve
```
Then visit: http://localhost:4000

## 📝 Future Content Updates

All content is stored in `_data/` folder:
- `_data/experience.yml` - Work history
- `_data/skills.yml` - Technical skills
- `_data/projects.yml` - Project portfolio
- `_data/education.yml` - Education background
- `_config.yml` - Site configuration and personal info

## 🎨 Customization

- Site title, name, contact info: `_config.yml`
- Resume sections visibility: `_config.yml` (resume_section_* settings)
- Avatar: `images/avatar.png` (currently using Nate.PNG)

## 📞 Contact Information on Site

Currently configured with:
- Email: sales@stride.build
- Website: www.stride.build
- GitHub: github.com/cohesivejones

You can update these in `_config.yml` under the "Resume settings" section.
