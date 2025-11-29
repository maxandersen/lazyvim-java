# Example of Neovim configuration for Java development with LazyVim

This configuration is shown in a few blog posts at <https://www.lorenzobettini.it>:

* The first part, which ends in the branch [first-blog-post](https://github.com/LorenzoBettini/lazyvim-java/tree/first-blog-post), is described in the blog post <https://www.lorenzobettini.it/2024/11/neovim-and-java-with-lazyvim-part-1-initial-configuration/>.
* The second part, which also ends in the branch [first-blog-post](https://github.com/LorenzoBettini/lazyvim-java/tree/first-blog-post), is described in the blog post <https://www.lorenzobettini.it/2024/12/neovim-and-java-with-lazyvim-part-2-ide-mechanisms/>.
* The third part, which ends in the branch [third-blog-post](https://github.com/LorenzoBettini/lazyvim-java/tree/third-blog-post), is described in the blog post <https://www.lorenzobettini.it/2025/01/neovim-and-java-with-lazyvim-part-3-dependencies-and-maven/>.
* The fourth part, which ends in the branch [fourth-blog-post](https://github.com/LorenzoBettini/lazyvim-java/tree/fourth-blog-post), is described in the blog post <https://www.lorenzobettini.it/2025/03/neovim-and-java-with-lazyvim-part-4-running-programs/>.

To test it without overriding your Neovim configuration:

```shell
git clone git@github.com:LorenzoBettini/lazyvim-java.git ~/.config/lazyvim-java
```

And then, to use it:

```shell
NVIM_APPNAME=lazyvim-java nvim
```

## Tips

- Make sure you are running `nvim` with Java 21 as JDT LS needs it, and a recent `npm` as json LS needs it in your path. Without it you will get errors.
- If you see popups/errors during startup or when opening your first Java project you can press ':' and type 'Snaks.notifier.show_history()` to see the errors.

One way of doing this in isolation to try out is with mise:

`NVIM_APPNAME=lazyvim-java mise x npm@lts java@lts -- nvim`
