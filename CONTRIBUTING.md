# Contributing guide

We welcome contributions to the peer review project. You can either [open an issue](https://github.com/redhat-documentation/peer-review/issues) for discussion, or submit an update using the steps below.

## Submitting an update

These instructions show how to submit an update using the command line. You may also use the GitHub web interface for the update. Whichever method you choose, the update should be submitted as a pull request.

Before you begin:

* You must have a GitHub account.
* You must have [set up an SSH key for your GitHub account](https://docs.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account).

The first time you contribute:

1. Fork the repository.

   From the main page of the [GitHub repository](https://github.com/redhat-documentation/peer-review), click **Fork** in the upper right corner.

2. Clone the forked repository locally.

   ```
   $ git clone git@github.com:<username>/peer-review.git
   ```

   If this command fails, be sure that you have [set up an SSH key for GitHub](https://docs.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account).

3. Navigate to the `peer-review` directory.

4. Set the upstream remote repository.

   ```
   $ git remote add -f upstream git@github.com:redhat-documentation/peer-review.git
   ```

To submit an update:

1. Fetch the latest changes.

   ```
   $ git fetch upstream
   ```

2. Check out a branch from upstream/master

   ```
   $ git checkout -b <new-branch> upstream/master
   ```

3. Make your edits.

   Add or edit files as needed.

4. Stage the changes for each file.

   ```
   $ git add <file-name>
   ```

5. Commit the changes.

   ```
   $ git commit -m "<descriptive-commit-message>"
   ```

6. Push the changes to your forked repository.

   ```
   $ git push origin HEAD
   ```

7. Open a pull request.

   Typically the previous command gives the URL to open a pull request. If not, you can open one from the [Pull requests](https://github.com/redhat-documentation/peer-review/pulls) tab of the GitHub UI.

After you submit a pull request, it will be reviewed by members of this project.

<!--
## Building the guide

You must have `asciidoctor` installed.

1. Navigate to the `peer_review_guide` directory.
2. Use the following command to build the guide:

   ```
   $ asciidoctor master.adoc
   ```

This generates a `master.html` file that you can now view in a browser.

## Contributing guidelines

See the [Contributing guidelines](GUIDELINES.adoc) for guidelines to follow when making an update.

-->
