# Graph models for household speaker recognition

This is a course project for SNA by Igor Fedorov and Evgeny Shabalin.

The speaker embedder is adopted from [CLOVA](https://github.com/clovaai/voxceleb_trainer) and we use VoxCeleb-1 for household simulation.

Our graph-based algorithm is an adaptation of [Links](https://arxiv.org/abs/1801.10123) for given scenario. Precisely, we discard the node-splitting part and operate only with enrichment & merging.

Our algorithm outperforms simple enroll enrichment in terms of average EER:

(0.272 - 0.196 - 0.175 for n=2, 0.415 - 0.387 - 0.299 for n=4, 0.565 - 0.455 - 0.401 for n=6 after 1000 simulations)
