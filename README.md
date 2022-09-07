# How to setup MERN project on github

***Please read the guide carefully and don't skip any parts without reading them. This guide is here to help mainly people new to the mern stack (or full-stack dev in general). Only move onto the next step once you have completed the sub-steps to the previous step!***

You can use this [guide](https://www.mongodb.com/languages/mern-stack-tutorial) to work through the full-stack, however it doesn't specify anything about ***pushing to github***. This is why this guide is here to help with that.

### **Starting from Scratch:**
1. Create main root directory (This will be your "project" folder. Either in terminal: `mkdir [project-name]` or manually)
   - Go into the created directory: `cd [project-name]`
3. Create client dir:
    - `npx create-react-app client`
    - Once React installs, delete the .git folder manually or look up command [`rm -rf .git`](https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/delete-local-git-repository-repo-command-windows-linux-rm#:~:text=If%20you're%20familiar%20with,files%20and%20folders%20it%20contains.)[^1][^2].
    - Once done, `cd` back out to root.
4. Now create a server dir (`mkdir server`)
    - Use this --> [MongoDB guide](https://www.mongodb.com/languages/mern-stack-tutorial)[^3] to setup the back-end.
5. Once the above points are complete, `cd` out to root dir
    - Use `git init` to initialize the local repo (for the entire project)
      - Now: `git add .` -> `git commit -m 'first commit'` -> `git remote add [remote_name] [YOUR_GH_REPO_URL]`
        - `git push [remote_name] master`[^4] -> You might be asked for username and password. Use gh username and password requires a personal access token (found in developer settings).[^5][^6]
6. You now have a full-stack app on GitHub CONGRATS!

P.S. REMEMBER TO SAVE THAT PERSONAL ACCESS TOKEN BECAUSE YOU HAVE TO REGEN EACH TIME YOU WANT TO SEE IT!!!

[^1]: https://stackoverflow.com/questions/61573115/rm-rf-equivalent-for-windows-powershell
[^2]: https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/delete-local-git-repository-repo-command-windows-linux-rm#:~:text=If%20you're%20familiar%20with,files%20and%20folders%20it%20contains.
[^3]: https://www.mongodb.com/languages/mern-stack-tutorial
[^4]: https://stackoverflow.com/questions/60152507/how-to-upload-a-full-stack-reactjs-nodejs-socketio-project-to-github-by-gi
[^5]: https://stackoverflow.com/questions/17659206/git-push-results-in-authentication-failed
[^6]: https://stackoverflow.com/questions/68775869/message-support-for-password-authentication-was-removed-please-use-a-personal
