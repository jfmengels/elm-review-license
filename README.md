# elm-review-license

Provides an [`elm-review`](https://package.elm-lang.org/packages/jfmengels/elm-review/latest/) rule to make sure you don't use packages with unapproved licenses.


## Provided rules

- [`NoUnapprovedLicense`](https://package.elm-lang.org/packages/jfmengels/elm-review-license/1.0.0/NoUnapprovedLicense) - Reports dependencies with unapproved licenses.


## Configuration

```elm
module ReviewConfig exposing (config)

import NoUnapprovedLicense
import Review.Rule exposing (Rule)

config : List Rule
config =
    [ NoUnapprovedLicense.rule
        { allowed = [ "BSD-3-Clause", "MIT" ]
        , forbidden = [ "GPL-3.0-only", "GPL-3.0-or-later" ]
        }
    ]
```


## Try it out

You can try the example configuration above out by running the following command:

```bash
elm-review --template jfmengels/elm-review-license/example
```
