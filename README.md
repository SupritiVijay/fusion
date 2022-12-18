Fine-Tuning fusion model for case-hold/logiqa dataset:

Setup for this project
- put pre-processed data into data folder
    - one dataset for text and one dataset for AMR data (generated by Spring AMR parser)
- put AMRBART model into amrbart folder (https://github.com/goodbai-nlp/AMRBART)
- update paths in scripts/run*.sh files

Other information:
- Spring is part of the project since we need the PENMANBartTokenizer (which is used by AMRBART).
- The fusion model fine-tuned on CaseHOLD can be found here: https://huggingface.co/niks883/fusion-case-hold
- The fusion model fine-tuned on LogiQA can be found here: https://huggingface.co/niks883/fusion-logiqa
- For other baselines models refere to this repository https://github.com/nschrack/baselines-mcqa

If you are using this GitHub repository, please cite our paper as follows:

```
@inproceedings{schrack-etal-2022-amr,
  author = {Schrack, Nikolaus and Cui, Ruixiang and López, Hugo A. and Hershcovich, Daniel},
  title = {Can {AMR} Assist Legal and Logical Reasoning?},
  booktitle = {Findings of the Association for Computational Linguistics: EMNLP 2022},
  publisher = {Association for Computational Linguistics},
  year = {2022},
  month = dec
}
```
