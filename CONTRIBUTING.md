# Contributing

Thanks for wanting to add something. This list is curated, not exhaustive, so most of what follows is about what gets left out and why.

Open a pull request that adds a single entry. If you have several to suggest, one PR each is easier to discuss than one PR with a batch, since I may want to take some and not others.

## What belongs here

Packages, tools, and applications that are built on Ink or that exist specifically to serve Ink apps. Components, hooks, frameworks, testing helpers, build tooling, and CLIs that people actually use.

What does not belong:

* General React libraries that happen to work in a terminal. If it has nothing to do with Ink, it goes on a React list.
* Terminal UI toolkits for other languages or other runtimes. Those are interesting, but they are not this list.
* Blog posts and tutorials, for now. I have not found enough good ones to justify a section, and a section with two links in it looks worse than no section.
* Anything abandoned. See below.

## The bar

Every entry has to clear all four of these:

1. **It is published and installable.** On npm, or a real application someone can run. A repo with source and no release is not usable yet.
2. **It works with a current Ink.** Ink is on v7 at the time of writing. Declaring `ink >=5` in peer dependencies is not the same as working on v7, and I will probably check. If it only supports v4 or older, it is not ready for this list.
3. **It is alive.** A commit or a release in the last twelve months, and the repo is not archived. Small and finished is fine. Small and abandoned is not.
4. **It is not already solved upstream.** Ink core and [Ink UI](https://github.com/vadimdemedes/ink-ui) between them cover spinners, progress bars, selects, multi-selects, text and confirm inputs, ordered and unordered lists, and quite a lot more. If your package does one of those things, tell me in the PR what it does that the first-party option does not. "It is a different implementation" is not enough on its own.

Then there is a popularity floor, which is a blunt instrument and I know it:

* **Applications and games: 100 stars.** This is borrowed straight from Ink's own showcase rule, so at least it is a number the ecosystem already recognizes.
* **Libraries, components, hooks, and tooling: 50 stars, or roughly 500 weekly npm downloads.** Either one is enough, not both. A component that does one narrow thing well can be the right answer for its niche and never get starred much, and downloads catch the packages people depend on quietly.

If your package is close to the line and clears everything else comfortably, say so in the PR and make the case. I would rather argue about one good entry than pretend the number is a law of nature.

There is one exception to all of the above. Anything linked from the [official Ink readme](https://github.com/vadimdemedes/ink) is in, no questions asked. Vadim and Sindre have already made the call, and I am not going to second guess the maintainers of the thing this list is about. That covers the useful components and hooks sections, the showcase of apps built with Ink, and the projects Ink itself is built on.

Practically, this means a package can be here on merit or on that inheritance, and you do not need to argue for the second kind. If it is on the Ink readme and missing from this list, that is a bug, so open a PR.

## Below the bar

New and promising things go in [`INCUBATING.md`](INCUBATING.md) instead of the readme. That file has no popularity floor, just the four requirements above. It is not a consolation prize, it is a queue, and I check it periodically to see what has grown.

Adding your own project there is fine and encouraged. My own Ink libraries are in that file, not in the readme, because they do not clear the floor either.

## Self promotion

Allowed, and you do not need to be coy about it. Same bar as everything else, no exceptions in either direction. My own packages are held to it, which is why they are in `INCUBATING.md` rather than the readme.

## Formatting

One line per entry:

```
- [name](https://github.com/user/repo) - Description of what it does.
```

The details matter more than they should, because this list follows the [Awesome guidelines](https://github.com/sindresorhus/awesome/blob/main/pull_request_template.md) and lint will complain:

* A hyphen separates the link from the description, with a space either side.
* The description starts with a capital letter and ends with a period.
* Keep it to one line. Say what the thing does, not why it is good. No taglines, no marketing.
* Link to the repository, not to npm, unless there is no repository.
* Use the project's own capitalization. It is `ink-text-input`, not `Ink Text Input`.
* Add the entry at the bottom of the section it belongs in.

If you are not sure which section, guess and say so in the PR. Sections are cheap to change.

## Removals

Please open an issue if something here has gone stale, broken against a current Ink, or been abandoned. Keeping bad entries out is the whole point of the list, and I will miss things.

## About AI

Use whatever tools you like, but read what you are submitting and make sure it is true. <!--I have had entries proposed for packages that do not exist and descriptions that confidently describe features the package does not have, which costs me more time to check than it saved you to generate.-->

Upstream Awesome does not accept AI generated lists at all, and this list intends to stay eligible.

## Code of conduct

Be decent to people. I will not write out the long version.
