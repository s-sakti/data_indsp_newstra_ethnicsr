# INDspeech07: INDspeech_NEWSTRA_EthnicSR

This is a collection of graphemically balanced and parallel speech corpora of four major Indonesian ethnic languages: Javanese, Sundanese, Balinese, and Bataks. It was developed in 2013 by the Nara Institute of Science and Technology (NAIST, Japan) [[Sakti et al., 2013](https://ieeexplore.ieee.org/document/6709907)]. The data has been used to develop Indonesian ethnic speech recognition in supervised [[Sakti et al., 2014](https://www.isca-speech.org/archive/sltu_2014/sakti14_sltu.html)] and semi-supervised learning [[Novitasari et al., 2020](https://aclanthology.org/2020.sltu-1.18/)] based on Machine Speech Chain framework [[Tjandra et al., 2020](https://ieeexplore.ieee.org/document/9020132)]. 

## Text and Speech Resources of Graphemically-balanced dataset

Raw text sources are collected from online newspapers and magazines of Javanese, Sundanese, Balinese, and Bataks. We then further processed the raw text sources to generate clean text corpora and selected 1000 sentences from cleaned text corpora of each language to be validated by the native speakers.

After that, we selected graphemically-balanced Sentences from the validated text data. A minimum set with a total of 225 sentences is produced using [the greedy search algorithm](https://www.internationalphoneticassociation.org/icphs-proceedings/ICPhS2003/papers/p15_3145.pdf). 

| Graphame | Javanese |  Sundanese |  Balinese | Bataks | 
|                    | #Units | Coverage | # Units | Coverage | # Units | Coverage | # Units | Coverage | 
| Mono-grapheme | 27 | 100% | 27 | 100% | 28 | 100% | 23 | 100% |  
| Left Bi-grapheme | 487 | 86.50% | 489 | 87.79% | 441 | 82.28% | 287 90.25% | 
| Right Bi-grapheme | 482 | 86.07% | 487 | 87.59% | 438 | 82.18% | 285 90.19% |  
| Tri-grapheme | 3269 | 53.99% | 3197 | 52.56% | 2796 | 53.35% | 1767 71.42% | 

Forty native speakers participated in the recording, 10 native speakers (5 males and 5 females) of each Javanese, Sundanese, Balinese, Bataks language, which originally came from ethnics of Java, Sunda, Bali, and North Sumatra. Then, each speaker was asked to read the prepared text of the 225 sentences. Each audio file is a single-channel 16-bit PCM WAV with a sample rate of 16 kHz.

## Text and Speech Resources of Parallel Indonesian-Ethnic languages dataset

In addition to graphemically balanced sentences, we created fifty sentences in Indonesian based on the travel expression. Those sentences were then translated into Javanese, Sundanese, Balinese, and Bataks languages by native speakers. 

| Languages | Sentences | 
| Indonesian | Apakah anda bersedia untuk makan dengan saya besok malam? | 
| Javanese | Opo kowe gelem mangan bareng aku sesuk bengi? |  
| Sundanese | Dupi anjeun sanggem kanggo tuang sareng abdi enjing wengi? | 
| Balinese | Napikeh mresidayang ragane buin mani peteng ngajeng sareng tiang? | 
| Bataks | Boha molo rap marjobut hita masogot bot ari? | 

Similar to the graphemically-balanced dataset, forty native speakers participated in the recording, 10 native speakers (5 males and 5 females) of each Javanese, Sundanese, Balinese, and Bataks language, which originally came from ethnics of Java, Sunda, Bali, and North Sumatra. Then, each speaker was asked to read the prepared text of the 100 sentences (50 Indonesian sentences and 50 ethnic language sentences). Each audio file is a single-channel 16-bit PCM WAV with a sample rate of 16 kHz.

## File Format

```
"Ind001_F_Bli_C_news_0065.wav" 
```

- Speaker ID: IndXXX
- Gender ID: F (female) or M (male)
- Ethnic ID: Jaw (Javanese), Snd (Sundanese), Bli (Balinese) or Btk (Bataks)
- Type ID: C (Clean) 
- Content ID: news (news sentences), traInd (Indonesian travel expression), or traEth (Ethnic travel expression).
- Utterance ID: XXXX 

Note:
The file with "traInd" and "traEth" on the same utterance ID XXXX are parallel utterances. 
```
"Ind001_F_Bli_C_traInd_0001.wav"
"Ind001_F_Bli_C_traEth_0001.wav"
```

## License

This data is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) International License (see LICENSE_CC-BY-NC-4.0.txt). You can use the data free for non-commercial purposes, but you have to cite our paper if your work uses our data in your publication. If you remix, transform or build upon the material, you must distribute your contributions under the same license as the original. Furthermore, you are not allowed to create a copy of this dataset and share it publicly in your own repository without our permission.

## Citation

Please cite the following papers:

[[Sani et al., 2012](doc/2012_ssakti_OCOCOSDA.pdf)]:

```
@inproceedings{sani-cocosda-2012,
    title = "Towards Language Preservation: Preliminary Collection and Vowel Analysis of {I}ndonesian Ethnic Speech Data",
    author = "Sani, Auliya and Sakti, Sakriani and Neubig, Graham and Toda, Tomoki and Mulyanto, Adi and Nakamura, Satoshi",
    booktitle = "Proc. Oriental COCOSDA",
    year = "2012",
    pages = "118--122"
    address = "Macau, China"
}
```
