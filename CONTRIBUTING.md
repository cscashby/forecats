> [!WARNING]
> If you see this, you are likely on the old `ha_integration` branch. This has now been merged back into `master`. Please ensure you submit PRs against `master`.
>
> If your work is based on ha_integration, rebase your branch onto master using the code below before creating a PR. Once rebased, open a PR against master. Thank you!
>
    ```bash
    git fetch upstream master
    git checkout ha_integration
    git rebase upstream/master
    git push -f origin ha_integration
    ```

# Contributing to Forecats

## How to Contribute

1. **Fork the repository** and create your branch from `master`.
2. **Make your changes** with a descriptive commit messages.
3. **Test your changes** to make sure nothing is broken.
4. **Submit a pull request** with a description of your changes.

## Testing

There are no unit tests atm. You are welcome to contribute some if you want (preferrably using pytest). Otherwise, you can locally test that everything still works fine with

```bash
    cd local_testing && uv run test.py
```

Note that this requires [uv](https://docs.astral.sh/uv/).

Please try running it on an HA server before submitting the PR.

## Guidelines

- If you change the automation template, make sure these changes are reflected in `models.py` and `local_testing/test.py` as well.
  
## Need Help?

If you have questions, open an issue or start a discussion.