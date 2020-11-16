# elm-review-license

Provides [`elm-review`](https://package.elm-lang.org/packages/jfmengels/elm-review/latest/) rules to REPLACEME.


## Provided rules

- [`NoUnapprovedLicense`](https://package.elm-lang.org/packages/jfmengels/elm-review-license/1.0.0/NoUnapprovedLicense) - Reports REPLACEME.


## Configuration

```elm
module ReviewConfig exposing (config)

import NoUnapprovedLicense
import Review.Rule exposing (Rule)

config : List Rule
config =
    [ NoUnapprovedLicense.rule
    ]
```


## Try it out

You can try the example configuration above out by running the following command:

```bash
elm-review --template jfmengels/elm-review-license/example
```
