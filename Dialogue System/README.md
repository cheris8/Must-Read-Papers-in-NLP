# Must-read paepers in Dialogue System

## Goal-oriented Dialogue System

*(NBT)* **Neural Belief Tracker: Data-Driven Dialogue State Tracking**. Nikola Mrkšić, Diarmuid Ó Séaghdha, Tsung-Hsien Wen, Blaise Thomson, Steve Young. ACL 2017.
- [paper](https://arxiv.org/abs/1606.03777.pdf)

*(SUMBT)* **SUMBT: Slot-Utterance Matching for Universal and Scalable Belief Tracking.** Hwaran Lee, Jinsik Lee, Tae-Yoon Kim. The 57th Annual Meeting of the Association for Computational Linguistics (ACL).
- [paper](https://arxiv.org/pdf/1907.07421.pdf.pdf)

## Non-goal-oriented Dialogue System

### Retrieve

*(Poly-encoder)* **Poly-encoders: Transformer Architectures and Pre-training Strategies for Fast and Accurate Multi-sentence Scoring.** Samuel Humeau, Kurt Shuster, Marie-Anne Lachaux, Jason Weston. ICLR 2020.
- [paper](https://arxiv.org/pdf/1905.01969.pdf)

### Generate

*(Speaker Model)* **A Persona-Based Neural Conversation Model.** Jiwei Li, Michel Galley, Chris Brockett, Georgios P. Spithourakis, Jianfeng Gao, Bill Dolan. ACL 2016.
- [paper](https://arxiv.org/pdf/1603.06155.pdf)

*(TransferTransfo)* **TransferTransfo: A Transfer Learning Approach for Neural Network Based Conversational Agents.** Thomas Wolf, Victor Sanh, Julien Chaumond, Clement Delangue. NeurIPS 2018 CAI Workshop.
- [paper](https://arxiv.org/pdf/1901.08149.pdf)

**Will I Sound Like Me? Improving Persona Consistency in Dialogues through Pragmatic Self-Consciousness.** Hyunwoo Kim, Byeongchang Kim, Gunhee Kim. EMNLP 2020 and ICLR 2020 BAICS workshop (Oral).
- [paper](https://arxiv.org/pdf/2004.05816.pdf)

**Don't Say That! Making Inconsistent Dialogue Unlikely with Unlikelihood Training.** Margaret Li, Stephen Roller, Ilia Kulikov, Sean Welleck, Y-Lan Boureau, Kyunghyun Cho, Jason Weston. ACL 2020.
- [paper](https://arxiv.org/pdf/1911.03860.pdf)

### Hybrid

*(RetNRef)* **Retrieve and Refine: Improved Sequence Generation Models For Dialogue.** Jason Weston, Emily Dinan, Alexander H. Miller. Proceedings of the 2018 EMNLP Workshop SCAI: The 2nd International Workshop on Search-Oriented Conversational AI
- [paper](https://arxiv.org/pdf/1808.04776.pdf)
- sequence generation model은 uninformative하고 unengaging한 짧고 일반적인(generic) 문장을 만들어내는 문제점 존재 / retrieval model은 구체적인 문맥으로 tuning이 불가능하다는 문제점 존재 => 결합하자!
- RetNRef : retrieval model의 output을 generative model의 일반적인 input과 concatenate => 모델 training => generate
    - generator : Seq2Seq : 2-layer LSTM with attention
    - retriever : Key-Value Memory Network (코사인 유사도 사용)
- ConvAI2 dataset

**Wizard of Wikipedia: Knowledge-Powered Conversational agents.** Emily Dinan, Stephen Roller, Kurt Shuster, Angela Fan, Michael Auli, Jason Weston. ICLR 2019.
- [paper](https://arxiv.org/pdf/1811.01241.pdf)

**Recipes for building an open-domain chatbot.** Stephen Roller, Emily Dinan, Naman Goyal, Da Ju, Mary Williamson, Yinhan Liu, Jing Xu, Myle Ott, Kurt Shuster, Eric M. Smith, Y-Lan Boureau, Jason Weston.
- [paper](https://arxiv.org/pdf/2004.13637.pdf)

**Neural Approaches to Conversational AI.** Jianfeng Gao, Michel Galley, Lihong Li.
- [paper](https://arxiv.org/pdf/1809.08267.pdf)
- Dialogue System 전반에 대한 교과서 같은 느낌

**Deep Retrieval-Based Dialogue Systems: A Short Review.** Basma El Amel Boussaha, Nicolas Hernandez, Christine Jacquin, Emmanuel Morin.
- [paper](https://arxiv.org/pdf/1907.12878.pdf)
- Retrieval-Based Dialogue System에 대한 연구를 정리해놓은 페이퍼

## Datasets

*(PERSONA-CHAT)* **Personalizing Dialogue Agents: I have a dog, do you have pets too?** Saizheng Zhang, Emily Dinan, Jack Urbanek, Arthur Szlam, Douwe Kiela, Jason Weston.
- [paper](https://arxiv.org/pdf/1801.07243.pdf)

**Training Millions of Personalized Dialogue Agents**. Pierre-Emmanuel Mazaré, Samuel Humeau, Martin Raison, Antoine Bordes. EMNLP 2018.
- [paepr](https://arxiv.org/pdf/1809.01984.pdf)

*(Dialogue NLI)* **Dialogue Natural Language Inference.** Sean Welleck, Jason Weston, Arthur Szlam, Kyunghyun Cho.
