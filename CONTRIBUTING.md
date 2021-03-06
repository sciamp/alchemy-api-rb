# Contributing to alchemy-api-rb

alchemy-api-rb is work of [several contributors](https://github.com/technekes/alchemy-api-rb/graphs/contributors). You're encouraged to submit [pull requests](https://github.com/technekes/alchemy-api-rb/pulls), [propose features and discuss issues](https://github.com/technekes/alchemy-api-rb/issues).

#### Fork the Project

Fork the [project on Github](https://github.com/technekes/alchemy-api-rb) and check out your copy.

```
git clone https://github.com/contributor/alchemy-api-rb.git
cd alchemy-api-rb
git remote add upstream https://github.com/technekes/alchemy-api-rb.git
```

#### Create a Topic Branch

Make sure your fork is up-to-date and create a topic branch for your feature or bug fix.

```
git checkout master
git pull upstream master
git checkout -b my-feature-branch
```

#### Bundle Install and Test

Ensure that you can build the project and run tests.

```
bundle install
ALCHEMY_API_KEY="this-is-my-40-character-key" bundle exec rake test
```

#### Write Tests

Try to write a test that reproduces the problem you're trying to fix or describes a feature that you want to build. Add to [spec/](spec/).

We definitely appreciate pull requests that highlight or reproduce a problem, even without a fix.

#### Write Code

Implement your feature or bug fix.

Ruby style is enforced with [Rubocop](https://github.com/bbatsov/rubocop), run `bundle exec rubocop` and fix any style issues highlighted.

Make sure that `ALCHEMY_API_KEY="this-is-my-40-character-key" bundle exec rake test` completes without errors.

#### Write Documentation

Document any external behavior in the [README](README.md).

#### Update Changelog

Add a line to [CHANGELOG](CHANGELOG.md) under *Next Release*. Make it look like every other line, including your name and link to your Github account.

#### Commit Changes

Make sure git knows your name and email address:

```
git config --global user.name "Your Name"
git config --global user.email "contributor@example.com"
```

Writing good commit logs is important. A commit log should describe what changed and why.

```
git add ...
git commit
```

#### Push

```
git push origin my-feature-branch
```

#### Make a Pull Request

Go to https://github.com/technekes/alchemy-api-rb/compare and select your feature branch. Click the 'Create pull request' button and fill out the form. Pull requests are usually reviewed within a few days.

#### Rebase

If you've been working on a change for a while, rebase with upstream/master.

```
git fetch upstream
git rebase upstream/master
git push origin my-feature-branch -f
```

#### Update CHANGELOG Again

Update the [CHANGELOG](CHANGELOG.md) with the pull request number. A typical entry looks as follows.

```
* [#13](https://github.com/technekes/alchemy-api-rb/pull/13): Adds targeted sentiment analysis endpoint - [@vaibhao90](https://github.com/vaibhao90) and [@johnallen3d](https://github.com/johnallen3d).
```

Amend your previous commit and force push the changes.

```
git commit --amend
git push origin my-feature-branch -f
```

#### Check on Your Pull Request

Go back to your pull request after a few minutes and see whether it passed muster with Travis-CI. Everything should look green, otherwise fix issues and amend your commit as described above.

#### Be Patient

It's likely that your change will not be merged and that the nitpicky maintainers will ask you to do more, or fix seemingly benign problems. Hang on there!

#### Thank You

Please do know that we really appreciate and value your time and work. We love you, really.
