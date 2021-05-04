## Instructions

### Directory structure (the important bits)
```
📁 assets
    📁 media
        📄 icon.png - (optional) add your website icon here
        📄 logo.png - (optional) add your logo here
📁 config
    📁 _default
        📄 config.yaml - define your site name and URL
        📄 languages.yaml - edit this for non-English or multilingual sites
        📄 menus.yaml - define your site menu
        📄 params.yaml - personalize your site
📁 content
    📁 authors - user profiles
        📁 admin - your username (can rename)
            📄 _index.md - your user profile
            📄 avatar.jpg - update with a photo of yourself or delete to not show any photo
    📁 home - your homepage - personalize the homepage with widgets
    📁 post
        📄 _index.md - (optional) an archive of blog posts
    📁 publication
        📄 _index.md - (optional) an archive of publications
    📁 projects
        📄 _index.md - (optional) an archive of projects
📁 data
    📄 page_sharer.toml - (optional) customize social sharing buttons
```

### Creating a new project/post

- Run the below command with the appropriate `--kind` of content you want to make, and the path you want it in
```
hugo new --kind post content/post/my_new_post_directory
```
- Edit `content/post/my_new_post_directory/index.md`. See [here](https://wowchemy.com/docs/content/) for full details
- Add and commit any changes to the source

### Push changes to the website
- If you have not already done so, run `hugo`. It will to build the webpage in the `public` directory
- Add and commit your changes
```
git add public/
git commit -m "Your commit message"
```
- Push just the `public/` folder to `gh-pages` branch
```
git subtree push --prefix=public origin gh-pages
```
---

- Template based on Academic theme's [Starter Research Group](https://github.com/wowchemy/starter-hugo-research-group)
- Documentation [here](https://wowchemy.com/docs/)