# @fforw/clumpomatic

Image filter based on jimp. Averages out square areas within a source image.

Uses a exponential distribution from the lowest amount for the largest clumb to the highest amount of smallest clumps.

## Usage

```sh
clumpomatic --size 4 --min 1000 --max 9000 --pow [p=3] <in> <out>
```

Will average a 4x4 square a thousand times and then continuing counting down sizes 3,2,1 to reach 9000 times for 1 and
an exponential (default cubic) curve.
