# Publishing Soulfly Dark

This extension contains only a theme; it does not need Rust or WebAssembly.

## Before submitting

1. Install this repository as a dev extension in Zed.
2. Select **Soulfly Dark** and check syntax highlighting, the interface,
   diagnostics, selections, and the integrated terminal.
3. Review the Zed screenshot in `assets/soulfly-dark.png`, embedded in the
   main README. To refresh it, use the ignored `screenshot-demo/` TypeScript
   project; its README contains local instructions.
4. Confirm that `extension.toml` has the intended version, author, and repository.
5. Commit the extension files on `main` and publish the public repository at
   `https://github.com/pridees/soulfly-dark-theme`.

## Submit to the Zed extension registry

Follow the official [publishing guide](https://zed.dev/docs/extensions/publishing/publishing-guide).

1. Fork `zed-industries/extensions` to your GitHub account and clone the fork.
2. Create a submission branch.
3. Add the public theme repository as an HTTPS submodule:

   ```sh
   git submodule add https://github.com/pridees/soulfly-dark-theme extensions/soulfly-dark-theme
   ```

4. Add this entry to the registry's `extensions.toml`:

   ```toml
   [soulfly-dark-theme]
   submodule = "extensions/soulfly-dark-theme"
   version = "1.0.0"
   ```

5. Run `pnpm sort-extensions` in the registry repository.
6. Confirm the submodule points to the same commit you tested in Zed,
   reachable on `main` in the public theme repository.
7. Commit, push the submission branch, and open a pull request against
   `zed-industries/extensions`. Include a screenshot and the manual checks.

The extension becomes available in Zed after the registry maintainers accept
and merge the pull request. Publishing the GitHub repository alone does not
publish the extension in Zed.

## Updates

Increment the manifest version, update the changelog, and push the tested commit.
Then update both the registry submodule pointer and the matching version in
`extensions.toml` through a new pull request.
