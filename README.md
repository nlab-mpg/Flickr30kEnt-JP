# Flickr30kEnt-JP
©2020, The University of Tokyo

Japanese translation of the Flickr30k Entities dataset presented in [our paper at LREC2020](http://www.lrec-conf.org/proceedings/lrec2020/pdf/2020.lrec-1.518.pdf).

Our dataset is based on the original [Flickr30k](http://shannon.cs.illinois.edu/DenotationGraph/) and [Flickr30k Entities](http://bryanplummer.com/Flickr30kEntities/) datasets. We do not own the copyrights of images, English captions, and annotations in these datasets. Please visit the authors' web pages and follow their instructions to download them.


**(2020 July) We are going to have [Multimodal English-Japanese Translation Task](https://nlab-mpg.github.io/wat2020-mmt-jp/) at [WAT2020](https://lotus.kuee.kyoto-u.ac.jp/WAT/WAT2020/index.html)!**

**(2021 August) We released the full translation of all captions in the original Flickr30k (check our v2 dataset).**  

## License
Our dataset is released under the [Creative Commons Attribution-ShareAlike (CC BY-SA) license](https://creativecommons.org/licenses/by-sa/4.0/legalcode).

## Dataset Description
We basically follow the same annotation rules as the Flickr30k Entities dataset.
You can find the text files named (image_id).txt corresponding to each image in Flickr30k. The files are encoded in the UTF-8 format. Each file has two lines (sentences) that correspond to the first two English captions for the same image in the Flickr30k Entities. 

We use the following notation for annotating phrases. 
```
n:[TAG PHRASES]
```
Above, n is the index of the corresponding phrase in the original English caption (starting from one), and TAG is exactly the same tag used there (refer to Flickr30k Entities datasets for details).

Below, we quote the first two lines of a file in the Flickr30k Entities and our corresponding Japanese file, as an example.

```
[/EN#18/people A child] in [/EN#19/clothing a pink dress] is climbing up [/EN#20/other a set of stairs] in [/EN#23/scene an entry way] .
[/EN#18/people A little girl] in [/EN#19/clothing a pink dress] going into [/EN#21/scene a wooden cabin] .
```
```
2:[/EN#19/clothing ピンクのワンピース]を着た1:[/EN#18/people 子供]が、4:[/EN#23/scene 玄関]の3:[/EN#20/other 階段]を上っている。
3:[/EN#21/scene 木造の小屋]の中に入りつつある、2:[/EN#19/clothing ピンクのワンピース]を着た1:[/EN#18/people 小さな女の子]。
```
For instance, the Japanese phrase "ピンクのワンピース" at the head of the first caption corresponds to the second phrase in the English caption, "a pink dress". Similarly, we can find that "木造の小屋" in the second caption corresponds to the third phrase in English, "a wooden cabin". 

Note that some tags in the original English captions do not appear in our Japanese translations when it is difficult to keep explicit phrase-to-phrase correspondences (see our paper for details).

## Reference
If you use this dataset, please cite the following paper ([pdf](http://www.lrec-conf.org/proceedings/lrec2020/pdf/2020.lrec-1.518.pdf)).

Hideki Nakayama, Akihiro Tamura, and Takashi Ninomiya, In Proceedings of The 12th Language Resources and Evaluation Conference, pp.4204-4210, 2020.
```
@InProceedings{nakayama-tamura-ninomiya:2020:LREC,
  author    = {Nakayama, Hideki  and  Tamura, Akihiro  and  Ninomiya, Takashi},
  title     = {A Visually-Grounded Parallel Corpus with Phrase-to-Region Linking},
  booktitle      = {Proceedings of The 12th Language Resources and Evaluation Conference},
  month          = {May},
  year           = {2020},
  address        = {Marseille, France},
  publisher      = {European Language Resources Association},
  pages     = {4204--4210},
}
```
## Acknowledgment
This project is supported by “Research and Development of DeepLearning Technology for Advanced Multilingual Speech Translation”, the Com-missioned Research of National Institute of Information and CommunicationsTechnology (NICT), JAPAN.  
