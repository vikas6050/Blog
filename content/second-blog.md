+++
title = 'Creating Blog Page in Github website using Hugo'
date = 2023-09-20T12:51:46+05:30

+++

# Creating a Website on GitHub with Hugo Server

If you're looking to create a static website and host it on GitHub, you're in the right place! GitHub Pages offers free hosting for static websites, and Hugo is a popular static site generator that can help you build a beautiful and responsive website quickly. In this tutorial, we'll walk you through the steps to create a website using Hugo and host it on GitHub Pages.

## Prerequisites

Before we begin, make sure you have the following prerequisites:

1. **GitHub Account**: If you don't have one, sign up for a GitHub account at [github.com](https://github.com).

2. **Git**: Install Git on your local machine. You can download it from [git-scm.com](https://git-scm.com/).

3. **Hugo**: Install Hugo on your local machine. You can download it from [gohugo.io](https://gohugo.io/).

## Step 1: Create a New GitHub Repository

1. Log in to your GitHub account.

2. Click the '+' icon in the upper-right corner and select "New Repository."

3. Fill in the repository name (e.g., "my-website") and add a brief description.

4. Choose the repository visibility (public or private). For GitHub Pages to work, the repository should be public.

5. Optionally, choose a license for your project.

6. Click the "Create repository" button.

## Step 2: Clone the Repository

Once your repository is created, you'll need to clone it to your local machine.

```bash
git clone https://github.com/your-username/my-website.git
cd my-website
```

Replace `your-username` with your GitHub username and `my-website` with your repository name.

## Step 3: Initialize Hugo

1. In your terminal, navigate to the project folder.

2. Initialize a Hugo site in your project folder:

```bash
hugo new site .
```

3. Choose a Hugo theme that you like. You can find themes at [themes.gohugo.io](https://themes.gohugo.io/). For example, to add the "Ananke" theme:

```bash
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
```

4. Configure your website by editing the `config.toml` file. Set your website title, author information, and any other desired settings.

## Step 4: Create Content

1. Create a new content page with Hugo:

```bash
hugo new posts/my-first-post.md
```

This command will generate a Markdown file for your first blog post.

2. Edit the Markdown file (e.g., `content/posts/my-first-post.md`) to add your content.

## Step 5: Build the Website

Generate the static HTML files for your website using Hugo:

```bash
hugo
```

This will create a `public` folder with the compiled website.

## Step 6: Commit and Push to GitHub

1. Add all the changes to Git and commit them:

```bash
git add .
git commit -m "Initial commit"
```

2. Push your changes to GitHub:

```bash
git push origin main
```

## Step 7: Configure GitHub Pages

1. Go to your GitHub repository's settings.

2. Scroll down to the "GitHub Pages" section.

3. Set the source branch to `main` (or `master`, depending on your default branch name).

4. Click "Save."

## Step 8: Access Your Website

After a few moments, your website should be live at `https://your-username.github.io/my-website/`. Replace `your-username` with your GitHub username and `my-website` with your repository name.

Congratulations! You've successfully created a website using Hugo and hosted it on GitHub Pages. You can now customize your website further, add more content, and explore Hugo's extensive features to make it uniquely yours. Happy coding!
