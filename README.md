# Fernexus

This is a project created so I can host a blog on github pages and learn some new things along the way.

## To run this project locally

1. Clone this repo down using git
2. `cd Fernexus`
3. `npm install`
4. `npm run start`

## Changes required to deploy this project to github pages

1. Create an ACTIONS_DEPLOY_KEY following git hub instructions
2. Update the pathPrefix everywhere so the github pages urls resolve when deployed

### To deploy

Create an annotated git tag and then push it to main.

```sh
git tag -a v0.0.1 -m "Dev only Release v0.0.1"
git push
```

after deploy is complete

```sh
git fetch
git tag
```

and view both the pushed tag and the tag created by the gh-page deploy

    v0.0.2  
    deploy-v0.0.2

This project is currently set to run build and deploy on a git push on the main branch.


## Project references

- https://www.11ty.dev/docs/config/#deploy-to-a-subdirectory-with-a-path-prefix
- https://www.rockyourcode.com/how-to-deploy-eleventy-to-github-pages-with-github-actions/
- https://keepinguptodate.com/pages/2019/06/creating-blog-with-eleventy/
- https://lea-tortay.com/articles/github-pages-eleventy/index.html
- https://github.com/peaceiris/actions-gh-pages?tab=readme-ov-file#%EF%B8%8F-set-ssh-private-key-deploy_key

## TODO's

- Change to using sass for styling
- Add any missing aria attributes
- Add caching