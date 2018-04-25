# Panlex-Lexicon-Extractor
The script is a tool to extract bilingual lexicon for pair of languages from the [Panlex Database](https://db.panlex.org/) released by [Panlex](https://panlex.org/).
# Extracted Lexicons (English-{target})

# Usage
The code is written is Python 2.7.
Download the required [file](https://drive.google.com/file/d/1tyACWPYrOQJ4m20dTjDPWtpX1XGYWtyf/view?usp=sharing) of Panlex language information. Put it under the folder of 'data'

Download the preprocessed SQLite file of Panlex database [here](https://drive.google.com/file/d/1WiAkuBOFt0oFARvA1OWb_YsxPIDcKigW/view?usp=sharing), uncompress and put it under the folder of 'data'

The script accepts 3-digit [ISO 639-3](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) language codes.
```
python panlex_bilingual_extract.py --source_language=spa\
				   --target_language=eng\
				   --output_directory=data/lexicons
```

# Citation
If you find the lexicon extractor useful, please cite the following paper: [Embracing non-traditional linguistic resources for low-resource language name tagging](http://www.aclweb.org/anthology/I17-1037)
```
@inproceedings{zhang2017embracing,
  title={Embracing non-traditional linguistic resources for low-resource language name tagging},
  author={Zhang, Boliang and Lu, Di and Pan, Xiaoman and Lin, Ying and Abudukelimu, Halidanmu and Ji, Heng and Knight, Kevin},
  booktitle={Proceedings of the Eighth International Joint Conference on Natural Language Processing (Volume 1: Long Papers)},
  volume={1},
  pages={362--372},
  year={2017}
}
```