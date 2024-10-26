This is the repository for my blog built using quarto and deployed using github pages.  The site is live at https://clabornd.github.io/dmcblog/

I wanted to learn to use quarto, and making a blog seemed like a fun way to do that!

An overview of how to make a blog like this is described in [quarto's docs](https://quarto.org/docs/websites/website-blog.html)

I deploy using [github actions](https://docs.github.com/en/actions), which I've found to be pretty user friendly and cool!  The actions I use specific to deploying quarto are being developed on the [quarto-dev github](https://github.com/quarto-dev/quarto-actions).  I use quarto-dev/quarto-actions/setup@v2 and quarto-dev/quarto-actions/publish@v2.  The latter creates an orphan branch that contains only the contents of the built webpage (see the gh-pages branch).  In the repo settings, I tell Github pages to serve the website from that branch.

[Linkspector](https://github.com/UmbrellaDocs/linkspector) is used to check if the links in my posts are still valid, since I link to a ton of random websites, wandb output, colab notebooks, etc.  They provide a nice github action to run the checks before building the site.

If you've somehow managed to make it here and actually read something I've posted, I'm flattered; and if you notice something factually incorrect or just generally wrong (which is ... possible), feel free to put in a pull request.