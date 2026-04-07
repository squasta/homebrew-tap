# homebrew-tap
Homebrew Tap of Stanislas tools

## What is Homebrew?

Package manager for macOS (or Linux), see more at https://brew.sh

## What is a Tap?

A third-party (in relation to Homebrew) repository providing installable
packages (formulae) on macOS and Linux.

See more at https://docs.brew.sh/Taps

## How do I install packages from here?

```sh
brew install squasta/tap/name
```

You can also only add the tap which makes formulae within it
available in search results (`brew search` output):

```sh
brew tap squasta/tap
```

Note: to clone the tap via SSH you will need to use:

```sh
brew tap squasta/tap https://github.com/squasta/homebrew-tap
```

While you may search across taps, it is necessary to always use
fully qualified name (incl. the `squasta/tap/` prefix)
when refering to formulae in external taps such as this one
outside of search.

## What packages are available?

With the following commands, you can install the latest version of each tool:
```sh
# Formulae
brew install squasta/tap/nc2cli-go


## Why should I install packages from this tap?

Formulae for the same squasta software may exist in other taps
or the [community-maintained main tap](https://github.com/Homebrew/homebrew-core).
This may raise a question of why would someone prefer one tap over the other.

The _community-maintained tap_ compiles squasta tools on Homebrew's own infrastructure, and builds it according to the local formulae definition.

Formulae _in this tap_ are maintained by me (squasta), which means that it distributes
the exact (byte-to-byte) same binaries which are also published in my github repos (but on macOS for example, after downloading it, you will need to get them out of MacOS quarantine)

 - Updating of formulae is automated, which means that updates become available as they're released.

### Why don't I maintain formulae in the `homebrew-core` (main tap)?

Homebrew's core team prefers to keep `homebrew-core` as community maintained and built from source to maintain consistency across vendors in terms of expectations around contents and updates. See [relevant discussion](https://discourse.brew.sh/t/maintenance-of-formulas-by-vendor/7649) for more information.
