turksfeat
===

Resources for [*Simple Speech Representation Learning from Perceptual Data*](https://github.com/Sleepwalking/prometheus-spark/blob/master/writings/simple-speech-representation-perceptual-data-hua-2019.pdf).


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
