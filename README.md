# Anderies Lab Website

Research group website built with [Hugo](https://gohugo.io/) and [Hugo Blox](https://hugoblox.com/).

## Prerequisites

- [Hugo](https://gohugo.io/installation/) (extended version)
- [Node.js](https://nodejs.org/) (for local CMS)

### macOS Installation

**With Homebrew:**
```bash
brew install hugo node
```

**With MacPorts:**
```bash
sudo port install hugo nodejs22
```

## Local Development

Start the Hugo development server:
```bash
hugo server
```

View the site at `http://localhost:1313/`

## Content Management System (Decap CMS)

This site includes [Decap CMS](https://decapcms.org/) for editing content through a web interface.

### Running the CMS Locally

1. Start Hugo server in one terminal:
   ```bash
   hugo server
   ```

2. Start the Decap CMS proxy server in another terminal (**must be run from the project directory**):
   ```bash
   npx decap-server
   ```

3. Access the CMS at `http://localhost:1313/admin/`

4. Click "Login" (no credentials needed for local development)

### What You Can Edit via CMS

| Content Type | Description |
|--------------|-------------|
| **Team Members** | Add/edit lab member profiles, roles, bios, and social links |
| **Publications** | Manage research publications with authors, DOIs, and abstracts |
| **Blog Posts** | Write news and blog posts |
| **Events** | Add conferences, talks, and other events |
| **Projects Page** | Edit the project slides/carousel |
| **Home Page** | Modify homepage sections |

### Content Structure

```
content/
├── _index.md              # Home page
├── authors/               # Team member profiles
│   └── {Name}/
│       ├── _index.md      # Profile data
│       └── avatar.jpg     # Profile photo
├── publication/           # Research publications
│   └── {slug}/
│       ├── index.md
│       └── cite.bib
├── post/                  # Blog posts
│   └── {slug}/
│       └── index.md
├── event/                 # Events
│   └── {slug}/
│       └── index.md
└── projects/              # Projects page
    └── index.md
```

### Adding Team Member Photos

Hugo Blox expects avatar images to be named `avatar.jpg` (or `avatar.png`) in each team member's folder. When uploading via CMS, you may need to rename the file to `avatar.jpg` in the folder.

## Manual Content Editing

You can also edit content directly in the markdown files:

- **Team Members:** `content/authors/{Name}/_index.md`
- **Publications:** `content/publication/{slug}/index.md`
- **Blog Posts:** `content/post/{slug}/index.md`
- **Events:** `content/event/{slug}/index.md`
- **Projects:** `content/projects/index.md`
- **Home Page:** `content/_index.md`

## Configuration

Site configuration files are in `config/_default/`:

- `hugo.yaml` - Hugo settings
- `params.yaml` - Site parameters and features
- `menus.yaml` - Navigation menus
- `module.yaml` - Hugo modules

## Building for Production

```bash
hugo
```

The built site will be in the `public/` directory.

## Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [Hugo Blox Documentation](https://docs.hugoblox.com/)
- [Decap CMS Documentation](https://decapcms.org/docs/)
