# PAL: Probing Audio Encoders via LLMs

This repository contains the code and other resources for the paper **PAL: Probing Audio Encoders via LLMs - A Study of Information Transfer from Audio Encoders to LLMs**.

**[Project Page](https://ta012.github.io/PAL/)** | **[Link to arXiv Paper]** (Link will be added upon publication) | **[Hugging Face Demo]** (Coming Soon)

---

### Abstract

> The integration of audio perception capabilities into Large Language Models (LLMs) has enabled significant advances in Audio-LLMs. Although application-focused developments, particularly in curating training data for specific capabilities e.g., audio reasoning, have progressed rapidly, the underlying mechanisms that govern efficient transfer of rich semantic representations from audio encoders to LLMs remain under-explored. We conceptualize effective audio-LLM interaction as the LLM's ability to proficiently probe the audio encoder representations to satisfy textual queries. This paper presents a systematic investigation on how architectural design choices can affect that. Beginning with a standard Pengi/LLaVA-style audio-LLM architecture, we propose and evaluate several modifications guided by hypotheses derived from mechanistic interpretability studies and LLM operational principles. Our experiments demonstrate that: (1) delaying audio integration until the LLM's initial layers establish textual context that enhances its ability to probe the audio representations for relevant information; (2) the LLM can proficiently probe audio representations exclusively through LLM layer's attention submodule, without requiring propagation to its Feed-Forward Network (FFN) submodule; (3) an efficiently integrated ensemble of diverse audio encoders provides richer, complementary representations, thereby broadening the LLM's capacity to probe a wider spectrum of audio information. All hypotheses are evaluated using an identical three-stage training curriculum on a dataset of 5.6 million audio-text pairs, ensuring controlled comparisons. Our final architecture, which incorporates all proposed modifications, achieves relative improvements from 10\% to 60\% over the baseline, validating our approach to optimizing cross-modal information transfer in audio-LLMs.

### Status

The code and models will be made available here soon. 

### Citation

If you find our work useful, please consider citing our paper:

```bibtex
@misc{alex2025pal,
    title        = {PAL: Probing Audio Encoders via LLMs - A Study of Information Transfer from Audio Encoders to LLMs},
    author       = {Tony Alex and Wish Suharitdamrong and Sara Atito and Armin Mustafa and Philip J. B. Jackson and Imran Razzak and Muhammad Awais},
    year         = {2025},
    eprint       = {},
    archivePrefix= {arXiv},
    primaryClass = {cs.SD}
}
