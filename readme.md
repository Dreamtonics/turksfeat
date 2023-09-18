turksfeat
===

Resources for [*Simple Speech Representation Learning from Perceptual Data*](https://github.com/Sleepwalking/prometheus-spark/blob/master/writings/simple-speech-representation-perceptual-data-hua-2019.pdf).

This database contains 3200 pairs (2700 for training and 500 for testing) of phonemes whose perceived similarity is rated by workers at Amazon Mechanical Turk. Each pair is rated by 5 workers on a 1-to-5 discrete opinion scale.

There is also a smaller database (screening set) with only 61 token pairs but each rated by 25 workers.

| Rating | Category | Description |
| --- | --- | --- |
| 5 | Identical | they sound the same |
| 4 | Very Similar | almost the same but distinguishable |
| 3 | Fair | similar but not the same |
| 2 | Poor | not so similar but related |
| 1 | Bad | completely different sounds |

Get VCTK
---

To use this database, you first need a copy of the [VCTK speech corpus](https://homepages.inf.ed.ac.uk/jyamagis/page3/page58/page58.html). Note that different license terms apply.


Data Format
---

* `vctk-pairs-screen.csv`, `vctk-pairs-test.csv`, `vctk-pairs-train.csv`

    speaker/speaker_utt1, time_start, time_end, speaker/speaker_utt2, time_start, time_end

    ### Example

    ```
    p225/p225_029,1.115,1.2,p225/p225_266,3.72,3.805
    p225/p225_301,1.725,1.825,p225/p225_165,3.77,3.875
    p226/p226_249,1.805,1.905,p226/p226_224,2.545,2.615
    p226/p226_249,1.545,1.65,p226/p226_144,3.495,3.625
    p226/p226_106,3.075,3.225,p226/p226_317,1.84,1.955
    ```

* `vctk-ratings-screen.csv`, `vctk-ratings-test.csv`, `vctk-ratings-train.csv`

    average, ratings[0], ratings[1], ratings[2], ...

    ### Example

    ```
    3.0,3,1,4,2,5
    3.6,2,5,3,5,3
    4.0,5,3,5,5,2
    4.6,5,5,4,4,5
    5.0,5,5,5,5,5
    ```

License
---

This database ("*turksfeat*") is made available under the Open Database License: [http://opendatacommons.org/licenses/odbl/1.0/](http://opendatacommons.org/licenses/odbl/1.0/). Any rights in individual contents of the database are licensed under the Database Contents License: [http://opendatacommons.org/licenses/dbcl/1.0/](http://opendatacommons.org/licenses/dbcl/1.0/).

In short: attribution and share-alike.
