<!--

if you update this file, then please run
`ln -f README.md _includes/content/README.md`
in terminal so the changes can be reflected on the site.
-->

# Recipes Styleguide

## Issues

Check the [issues page](https://github.com/moderndeveloper/recipes-styleguide/issues) on GitHub to see what needs to be done

## Development Process

### Getting started

1.  Fork the main [GitHub](https://github.com/moderndeveloper/recipes-styleguide) repo to your GitHub
2.  Clone the repository onto your computer

    ``` bash
    cd ~/YourDevelopmentDir
    git clone git@github.com:{your-github-username}/recipes-styleguide.git
    ```
3.  Look for an issue to solve on the GitHub Issues page
4.  Once you've found an issue you will work on, assign yourself to the issue (so no one else starts on that issue)
5.  Checkout a new branch to start work on your issue.

    ``` bash
    git checkout -b feature/{name-of-feature}
    ```

6.  Once you've finished your work, commit it, and push it
    1.  commit your work

        ``` bash
        git commit -a
        ```

    2.  your commit message should look something like the following

        ```
        Add {Name of feature}

        {A short description of what you did in the feature}
        ```

        an example of a good commit message would look something like this

        ```
        Add buttons

        1. Add documentation for button
        2. Add buttons.scss to ui-framework
        ```

        **NOTE:** Only write a high level overview of what you did,
        notice they didn't describe where `buttons.scss` was imported in
        ui-framework because that kind of information can be inferred if you work in this codebase.

   3.  push your branch to GitHub

       ``` bash
       git push origin HEAD
       ```

7.  Submit a Pull Request on GitHub
    1.  goto your fork of the UI Styleguide on GitHub
    2.  click the **Pull Request** button
    3.  make sure the
        1.  **base fork** is set to `moderndeveloper/recipes-styleguide`
        2.  **base** is set to `master`
        3.  **head fork** is set to `{your-github-user-name}/recipes-styleguide`
        4.  **compare** is set to your `feature/{name-of-feature}`
    4.  at the bottom of your description add

        ```
        @lifeiscontent ready for review
        ```

        so [**@lifeiscontent**](https://github.com/lifeiscontent) can review your work.

8.  Once your reviewer has finished reviewing and there is feedback you must fix your feature to satisfy requirements of the feature otherwise if everything is good, it will be merged into the master branch

### Continuing your efforts

You can keep your repository up to date by running the following command.

``` bash
git checkout master # if you're not on master
git pull --ff-only
```

then follow from step 3 in the **Getting started** section
