## Step 1: Create a branch

_Welcome to this course about the feature branch workflow! :wave:_

### What is the feature branch workflow?

The [feature branch workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow) is a Git workflow where all feature development is done in a dedicated branch (also known as a **feature branch**), instead of the `main` branch.

### Why use the feature branch workflow?

:muscle: **No broken code in `main`**: The encapsulation of features into dedicated branches makes it easy for developers to work on features without disturbing the main codebase. Thus, the `main` branch will never contain broken code.

:busts_in_silhouette: **Easy to collaborate**: The compartmentalization of feature branches makes it easy for multiple developers to work on features without interfering others. Without using branches, developers may resort to modifying the main codebase directly. As a result, developers may write code that breaks ongoing features done by others.

Feature branching also makes it possible to use **pull requests**. They give developers an opportunity to receive feedback and approval on their feature before being merged into the `main` branch.

:sparkles: **Popularity**: The core idea of the feature branch workflow is used by many other Git workflows, such as: [GitHub flow](https://docs.github.com/en/get-started/using-github/github-flow) and [forking workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow).

### :keyboard: Activity: Create a local feature branch

Congratulations, you created a startup! :tada:

With a group of friends, you co-founded DataWizard :magic_wand:, an interactive dashboard. Excited to showcase your startup, your team made a cool website, which can be viewed under [`website.md`](/website.md).

One day, you realize the website has a typo! :exploding_head: Can you find the typo? (Hint: Pyton or Python?)

Embarrassed, you want to fix the typo quickly before the world finds out. Worried that your fix may break the website on the `main` branch, you decide to try out the feature branch workflow.

1. Open this page in a new browser tab, and work on the steps in your second tab while you read the instructions in this tab.
2. Clone this repository onto your local computer and navigate to the project directory.

> [!TIP]
> You may wish to refer to this [guide](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) for more details on cloning a repository.

3. Create a new branch called `fix-typo` and switch to the new branch. The `fix-typo` branch will be your **feature branch** for fixing the typo. In this case, the branch name must be `fix-typo` to trigger the course workflow.

```
# Create a branch called `fix-typo`
git branch fix-typo

# Switch to branch `fix-typo`
git checkout fix-typo
```

> [!TIP]
> As the above two commands are often used together, you can combine both into a single command:
>
> ```
> git checkout -b fix-typo
> ```

4. Push the `fix-typo` branch to the [remote repository](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories) you cloned from on GitHub.

```
git push origin fix-typo
```

> [!NOTE]
> The above command follows the following format:
>
> ```
> git push <remote> <branch>
> ```
>
> where `<remote>` is the name of the remote connection pointing to a remote repository and `<branch>` is the specified local branch to push. Essentially, the above command pushes the local `fix-typo` branch to the repository you cloned from, which is pointed to by the remote connection named [`origin`](https://www.geeksforgeeks.org/git-origin-master/).

5. Return to the GitHub repository page and navigate to the **< > Code** tab in the header menu of your repository.

<img src="../../images/code-tab.png" alt="Code Tab" width="400">

6. Click on the **main** branch drop-down. You will see your new `fix-typo` branch displayed in the drop-down.

<img src="../../images/branch-dropdown.png" alt="Branch Dropdown" width="350">

7. Click on the **fix-typo** branch in the drop-down to switch to the new feature branch. The branch drop-down bar will reflect your new branch and display the new branch name.

<img src="../../images/fix-typo-branch.png" alt="fix-typo Branch" width="650">

8. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.
