# Website Maintenance Guide

Hello! This guide will help you manage and update the website.

## Initial Setup

1. **Clone the Repository**
   ```bash
   git clone git@github.com:shambhaviip/shambhaviip.github.io.git
   cd shambhaviip.github.io
   ```

2. **Install Hugo**
   - For Mac: `brew install hugo`
   - For Windows: Download from https://gohugo.io/installation/

## Making Changes

You'll mainly work with two things:

### 1. Content Directory (`content/`)
- This is where all the blog posts and gallery images live.
- Each folder here represents a section of the website
- Files are in Markdown format (`.md`) - it's like writing a simple text document
- You can edit these files with any text editor (VS Code, Notepad++, etc.)

### 2. Configuration (`hugo.yaml`)
- This file controls the website's settings
- You can edit things like:
  - Website title
  - Social media links
  - Navigation menu
  - Theme settings

## Workflow

1. **Before Making Changes**
   ```bash
   git pull origin main
   ```
   This gets the latest updates

2. **Preview Your Changes**
   ```bash
   hugo server
   ```
   - Visit http://localhost:1313 in your browser
   - The preview updates automatically as you make changes
   - Press Ctrl+C to stop the preview

3. **Build the Website**
   ```bash
   hugo build -d docs
   ```
   This creates the final website in the `docs/` folder

4. **Save Your Changes**
   ```bash
   git add .
   git commit -m "Describe your changes here"
   git push origin main
   ```

## Tips
- Always pull before making changes
- Preview your changes locally before pushing
