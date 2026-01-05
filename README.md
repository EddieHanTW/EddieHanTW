hi, i'm eddie 👋

second-year MS student at NTU CSIE. my research is somewhere in the intersection of efficient inference and multimodal understanding — basically trying to make vision-language models less of a compute hog without sacrificing too much on the capability side.

---

**what i'm working on lately:**

- adaptive visual token compression: VLMs generate way too many visual tokens. most of them aren't useful for a given query. i've been experimenting with attention-based pruning and token merging strategies that reduce compute by 40-60% with acceptable accuracy loss

- multimodal RAG: retrieval-augmented generation feels underexplored for vision tasks. been building tooling for evaluating how well VLMs can leverage retrieved visual context

- fine-tuning at scale (well, at "one grad student with one GPU" scale): LoRA/QLoRA recipes for LLaVA, Phi-3-vision, BLIP-2 that actually fit in 24GB VRAM

**background:**

undergrad was at NTU EE. spent most of it doing CV-adjacent stuff — object detection, image segmentation, that era. got pulled into the LLM world during COVID when everyone was suddenly training language models on whatever GPU they could get. the multimodal side felt like a natural landing spot since i already understood the vision stack.

took a year before starting my MS to work at a local startup doing document understanding. that experience made me realize how bad off-the-shelf VLMs are for real document parsing — charts, tables, mixed layouts. still thinking about that problem.

**things i find interesting that aren't research:**

hiking in the central mountain range when the weather cooperates. trying to learn Hakka (my grandparents spoke it, i can barely follow a conversation). reading about Byzantine history for reasons i can't fully explain.

---

**languages / tools:**

Python mostly. PyTorch. some JAX when the paper i'm reading only has JAX code. occasional Rust when i need something fast and deterministic. know enough C++ to debug CUDA issues but not enough to write anything from scratch.

---

*open to discussing research ideas, paper recommendations, or collaboration — just open an issue or something*

---

<details>
<summary>some papers i've found genuinely useful (not a comprehensive list, just things i keep coming back to)</summary>

- [LLaVA-1.5](https://arxiv.org/abs/2310.03744) — still a solid baseline, surprisingly hard to beat with tricks
- [ToMe](https://arxiv.org/abs/2210.09461) — token merging in ViTs, simple idea that holds up well
- [BLIP-2](https://arxiv.org/abs/2301.12597) — the Q-Former design is still interesting
- [LLaVA-NeXT](https://llava-vl.github.io/blog/2024-01-30-llava-next/) — dynamic resolution handling
- [InternVL2](https://internvl.github.io/) — the multi-scale approach makes a real difference
- the LoRA paper obviously ([Hu et al. 2021](https://arxiv.org/abs/2106.09685))

</details>
