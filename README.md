# Nathan Jones - Professional Resume

*Lead Consulting Software Developer with 15+ years of experience*

This repository contains my professional resume website built with Jekyll and hosted on GitHub Pages.

## 🌐 Live Site
The site will be available at: **[drnatejones.com](https://drnatejones.com)**

## 🚀 GitHub Pages Setup

### Step 1: Push to GitHub
```bash
git push origin master
```

### Step 2: Enable GitHub Pages
1. Go to your repository settings on GitHub (https://github.com/cohesivejones/cohesivejones/settings/pages)
2. Navigate to "Pages" section in the left sidebar
3. Under "Source", select the `master` branch (or `main` if that's your default)
4. Click "Save"

### Step 3: Configure Custom Domain (drnatejones.com)
1. In the GitHub Pages settings, add `drnatejones.com` to the "Custom domain" field
2. The CNAME file is already configured in this repository
3. In your domain registrar (where you manage drnatejones.com), add these DNS records:
   
   **A Records** pointing to GitHub Pages IPs:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
   
   **CNAME Record** (optional, for www subdomain):
   - Host: `www`
   - Points to: `cohesivejones.github.io`

4. Wait for DNS propagation (can take up to 24-48 hours, but usually faster)
5. Once the custom domain is verified, enable "Enforce HTTPS" in the GitHub Pages settings

## 🛠️ Local Development

To test locally, run the following in your terminal:

1. Install dependencies: `bundle install`
2. Start Jekyll server: `bundle exec jekyll serve`
3. Open your browser to `http://localhost:4000`

## 🐳 Running with Docker

To test locally with docker, run the following in your terminal:

1. `docker image build -t resume-template .`
2. `docker run --rm --name resume-template -v "$PWD":/home/app --network host resume-template`

## 📝 Updating Content

### Experience
Edit `_data/experience.yml` to update work history

### Skills
Edit `_data/skills.yml` to update technical skills

### Projects
Edit `_data/projects.yml` to update project portfolio

### Education
Edit `_data/education.yml` to update education information

### Personal Information
Edit `_config.yml` to update:
- Name and title
- Contact information
- Social media links
- Site configuration

### Avatar Image
Replace `images/avatar.png` with your own image

## 📋 Content Source
Resume content populated from RESUME.pdf and RESUME.docx

## 🙏 Credits
This site uses the [Resume Template](https://github.com/jglovier/resume-template) by Joel Glovier, customized for Nathan Jones.

## 📄 License
The template is licensed under the MIT license. [See project license.](LICENSE)
