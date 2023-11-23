# Natural Language Processing Project

Please see the uploaded Project_Report.pdf for a detailed report. Please see the link below for the original paper and code by Shane Storks: https://github.com/sled-group/Verifiable-Coherent-NLU

Verifiable-Coherent-NLU
Shared repository for TRIP dataset for verifiable NLU and coherence measurement for text classifiers. Covers the following publications in Findings of EMNLP 2021:
1. Shane Storks, Qiaozi Gao, Yichi Zhang, and Joyce Chai. (2021). [Tiered Reasoning for Intuitive Physics: Toward Verifiable Commonsense Language Understanding](https://arxiv.org/abs/2109.04947). In _Findings of EMNLP 2021_.
2. Shane Storks and Joyce Chai. (2021). [Beyond the Tip of the Iceberg: Assessing Coherence of Text Classifiers](https://arxiv.org/abs/2109.04922). In _Findings of EMNLP 2021_.

Please contact [Shane Storks](http://scr.im/sstorks) with any questions.

Setting up the environment
Part 1: use requirements.txt to create a conda environment
conda create --name test_env --file requirements.txt
conda activate test_env
python -m spacy download en_core_web_sm
pip install smart-open mkl-random torch huggingface-hub smart-open mkl-fft
Part 2: install the environment into jupyter (http://echrislynch.com/2019/02/01/adding-an-environment-to-jupyter-notebooks/)
pip install ipykernel
ipython kernel install --user --name=test_env
Part 3: activate your conda environment
conda activate test_env
Description
See Verifiable-Coherent-NLU.ipynb and Visualization folder for our code.


## Cite
If you use our code or models in your work, please cite one of our following papers from Findings of EMNLP 2021:
```
  @misc{storks2021tiered,
        title={Tiered Reasoning for Intuitive Physics: Toward Verifiable Commonsense Language Understanding}, 
        author={Shane Storks and Qiaozi Gao and Yichi Zhang and Joyce Chai},
        year={2021},
        booktitle={Findings of the Association for Computational Linguistics: EMNLP 2021},
        location={Punta Cana, Dominican Republic},
        publisher={Association for Computational Linguistics},
  }
```

```
  @misc{storks2021tip,
        title={Beyond the Tip of the Iceberg: Assessing Coherence of Text Classifiers}, 
        author={Shane Storks and Joyce Chai},
        year={2021},
        booktitle={Findings of the Association for Computational Linguistics: EMNLP 2021},
        location={Punta Cana, Dominican Republic},
        publisher={Association for Computational Linguistics},
  }
```

Additionally, please consider citing [Conversational Entailment](https://sled.eecs.umich.edu/post/resources/conversation-entailment/) and [ART](https://github.com/allenai/abductive-commonsense-reasoning), which are used in experiments from the latter paper (and included in this repo):
```
  @inproceedings{zhang-chai-2010-towards,
      title = "Towards Conversation Entailment: An Empirical Investigation",
      author = "Zhang, Chen  and
        Chai, Joyce",
      booktitle = "Proceedings of the 2010 Conference on Empirical Methods in Natural Language Processing",
      month = oct,
      year = "2010",
      address = "Cambridge, MA",
      publisher = "Association for Computational Linguistics",
      url = "https://aclanthology.org/D10-1074",
      pages = "756--766",
  }
```

```
  @inproceedings{
      bhagavatula2020abductive,
      title={Abductive Commonsense Reasoning},
      author={Chandra Bhagavatula and Ronan Le Bras and Chaitanya Malaviya and Keisuke Sakaguchi and Ari Holtzman and Hannah Rashkin and Doug Downey and Wen-tau Yih and Yejin Choi},
      booktitle={International Conference on Learning Representations},
      year={2020},
      url={https://openreview.net/forum?id=Byg1v1HKDB}
  }
```
