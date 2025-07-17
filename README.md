# kaah

kaah_news

## Article Pages

The project now includes individual article pages that can be placed in `content/articles`. Each article page is a Markdown file that will be processed when the site is generated. Use the following frontmatter in each article to set the title and publication date:

```markdown
---
title: "Article Title"
date: "2024-01-01"
---
```

Write the rest of the article content below the frontmatter in standard Markdown.

## Footer Design

The footer is located in `layouts/partials/footer.html`. It contains links to important pages and copyright information. Update the file if you want to add new links or customize the layout.

## Adding Images

Place images in the `static/images` directory. Reference them in your Markdown using the relative path, for example:

```markdown
![Alt text](/images/example.png)
```

Images placed in `static/images` will automatically be copied to the final site when you build.

## Customizing Colors

You can customize the site's colors by editing the CSS variables defined in `static/css/theme.css`. For example, to change the main accent color, update the `--accent` variable:

```css
:root {
  --accent: #00aaff; /* Replace with your preferred color */
}
```

## Running Locally

To preview the site locally, install the dependencies and start the development server:

```bash
npm install
npm run dev
```

The site will be available at `http://localhost:3000`. Changes to Markdown, layouts, or assets will reload automatically.
